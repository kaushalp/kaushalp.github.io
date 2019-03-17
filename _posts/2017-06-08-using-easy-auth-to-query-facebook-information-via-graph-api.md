---
id: 1845
title: 'Azure App Service: Using Easy Auth to query Facebook information via Graph API'
date: 2017-06-08T03:12:32+00:00
author: kaushal
layout: post
guid: https://blogs.msdn.microsoft.com/kaushal/?p=1845
permalink: /2017/06/08/using-easy-auth-to-query-facebook-information-via-graph-api/
opengraph_tags:
  - |
    <meta property="og:type" content="article" />
    <meta property="og:title" content="Azure App Service: Using Easy Auth to query Facebook information via Graph API" />
    <meta property="og:url" content="https://blogs.msdn.microsoft.com/kaushal/2017/06/08/using-easy-auth-to-access-facebook-information-using-graph-api/" />
    <meta property="og:site_name" content="Unleashed" />
    <meta property="og:description" content="On 8th August 2016, Facebook ended support FQL (Facebook Query Language). Here is a screenshot of the messaging from their site Facebook Query Language (FQL) Reference So they are encouraging the developers to use the GraphAPI to query the information. In this post we will cover on how to do this. Pre-Requisites Create an Azure..." />
    <meta property="og:image" content="https://msdnshared.blob.core.windows.net/media/2017/06/image_thumb192.png" />
    <meta name="twitter:card" content="summary" />
    <meta name="twitter:title" content="Azure App Service: Using Easy Auth to query Facebook information via Graph API" />
    <meta name="twitter:url" content="https://blogs.msdn.microsoft.com/kaushal/2017/06/08/using-easy-auth-to-access-facebook-information-using-graph-api/" />
    <meta name="twitter:description" content="On 8th August 2016, Facebook ended support FQL (Facebook Query Language). Here is a screenshot of the messaging from their site Facebook Query Language (FQL) Reference So they are encouraging the developers to use the GraphAPI to query the information. In this post we will cover on how to do this. Pre-Requisites Create an Azure..." />
    <meta name="twitter:image" content="https://msdnshared.blob.core.windows.net/media/2017/06/image_thumb192.png" />

categories:
  - accesstoken
  - Authentication
  - Authentication/Authorization
  - Authorization
  - Azure
  - Azure App Service
  - Azure Web App
  - Azure Websites
  - Easy Auth
  - facebook
  - FQL
  - Graph Api
  - Web App
  - X-MS-TOKEN-FACEBOOK-ACCESS-TOKEN
---
On **8th August 2016**, Facebook ended support **FQL** (*Facebook Query Language*). Here is a screenshot of the messaging from their site [Facebook Query Language (FQL)](https://developers.facebook.com/docs/reference/fql/)


![FQL Announcement](https://kaushalp.github.io/wp-content/uploads/2017/06/image192.png){:class="img-responsive"}

So they are encouraging the developers to use the **GraphAPI** to query the information. In this post we will cover on how to do this.

## Pre-Requisites

  * Create an Azure Web App and configure **Facebook** Authentication. This will require creating an **App ID** & **App Secret**. Refer this URL:  [How to Configure Facebook authentication](https://docs.microsoft.com/en-us/azure/app-service-mobile/app-service-mobile-how-to-configure-facebook-authentication) .
  * In the Azure Portal, under **Facebook Authentication Settings** select the *scopes* (or *permissions*) to access the required data.
  * I created a ASP.NET MVC 5 application with default authentication set to **Individual User Accounts**.

### Determining the scopes required to query the Facebook data

Facebook provides [Graph API Explorer](https://developers.facebook.com/tools/explorer/), which allows the users to test, create and debug their graph API calls. Using this the users can generate a **accesstoken** with specific scope. Using this token, the users can call the Facebook GraphApi and review the results.
Here is a screenshot of the UI:

![Facebook Graph API Explorer](https://kaushalp.github.io/wp-content/uploads/2017/06/image194.png){:class="img-responsive"}

### Create a Function to call an external Endpoint

The below **``RequestResponse()``** method takes an URL as input. Using the **``HttpWebRequest``** method, we call the URL and return the response.

```csharp
private string RequestResponse(string pUrl)
{
	HttpWebRequest webRequest = System.Net.WebRequest.Create(pUrl) as HttpWebRequest;
	webRequest.Method = "GET";
	webRequest.ServicePoint.Expect100Continue = false;
	webRequest.Timeout = 20000;

	Stream responseStream = null;
	StreamReader responseReader = null;
	string responseData = "";
	try
	{
		WebResponse webResponse = webRequest.GetResponse();
		responseStream = webResponse.GetResponseStream();
		responseReader = new StreamReader(responseStream);
		responseData = responseReader.ReadToEnd();
	}
	catch (Exception exc)
	{
		Response.Write("<br /><br />ERROR : " + exc.Message);
	}
	finally
	{
		if (responseStream != null)
		{
			responseStream.Close();
			responseReader.Close();
		}
	}
	return responseData;
}
```

### Calling the Facebook Graph Api

The below **``CallFacebookGraphApi()``** method code takes 3 inputs, all of which are of type string.

  1. **id** – This is the path that will be called. For example “me/feed”
  2. **fields** – this is the query string parameters that needs to be provided with the **id** above.
  3. **accesstoken** – this is the value of the **``X-MS-TOKEN-FACEBOOK-ACCESS-TOKEN``** header, that gets generated upon successful user login. This is used to authorize the GraphAPI call.

using the above 3 parameters we create a URL and call the **``RequestResponse()</span>``** method we created earlier.

```csharp
private string CallFacebookGraphApi(string id, string fields, string accessToken)
{
	string fbGraphiApiRequest = "https://graph.facebook.com/" + id + "?" + fields + "&access_token=" + accessToken;
	string response = RequestResponse(fbGraphiApiRequest);
	if (response == "")
	{
		response="<br /><br />Error while accessing the FB Graph API";
	}
	string resJson = response.Replace(@"\", string.Empty);
	var obj = JsonConvert.DeserializeObject(resJson);
	string formattedJson = JsonConvert.SerializeObject(obj, Formatting.Indented);
	return formattedJson;
}
```


### Fetching results from Facebook

Here we have a **``ActionResult``** Facebook, where we pass the parameters to the **``CallFacebookGraphApi()``** method we created above.

```csharp
public ActionResult Facebook()
{
	if(User.Identity.IsAuthenticated)
	{
		string accessToken = this.Request.Headers["X-MS-TOKEN-FACEBOOK-ACCESS-TOKEN"];
		// Retrieving the users details
		string myFields = "fields=first_name,last_name,middle_name,birthday,currency,email";
		string myJsonResponse = CallFacebookGraphApi("me", myFields, accessToken);
		ViewBag.Me = myJsonResponse;
	}
	return View();
}
```

I have deployed a working version of the code on one of my web apps (**Azure App Service**). You can see it working here: [https://easyauthkaushal-staging.azurewebsites.net](https://easyauthkaushal-staging.azurewebsites.net "https://easyauthkaushal-staging.azurewebsites.net")

This code is published on Github. You may fork it from here: [https://github.com/kaushalp/Facebook-GraphApi-with-EasyAuth](https://github.com/kaushalp/Facebook-GraphApi-with-EasyAuth "https://github.com/kaushalp/Facebook-GraphApi-with-EasyAuth")

HTH,  
Kaushal
