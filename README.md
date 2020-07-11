## K2 OneDrive Connector

This connector for K2 Cloud integrates with Microsoft OneDrive. It allows you to download and upload files, copy, move, and delete files, manage folders, and search for files and folders.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

# Features

  - Download and upload files
  - Search for files and folders
  - Update and delete files and folders
  - Note that this connector does not support tagging, e.g. the setting or retrieving of metadata, on files and folders. The other cloud storage connectors, such as Google Drive, Box, and Dropbox support tagging.

Note that while the .js or .jssp file can be modified, this is minified/bundled JavaScript and it is not recommended that you modify the files directly. Please log tickets using the [K2 Partner and Customer Portal](https://portal.k2.com) and log any feature requests on our [Ideas portal](https://ideas.k2.com/ideas).

## Getting the OneDrive Connector to work in your K2 environment

Before you see SmartObjects and run methods on them, you must do the following:

 - Create an Azure App in your Azure tenant
 - Assign permissions (Application and/or Delegated) to the app so it has the necessary permissions in Microsoft Graph to work from K2.
 - Create a secret for your app and copy the secret and the ID of the app for configuring an OAuth resource in K2
 - Create an OAuth Resource Type in K2 Management
 - Create an OAuth Resource in K2 Management based on the new resource type
 - Create a OneDrive service type with the bundled .js or .jssp file
 - Create a service instance for the type using the OAuth resource you created

 ### Creating the Azure App and Adding Permissions
 
 Create a new app in Azure by browsing to **Azure Active Directory > App registrations**. Give it a name like **K2 for OneDrive**. Once you have the app created, make a note of its Application ID. This is the app's client ID that you'll use when you create the OAuth resource in K2.

 Configure the Redirect URI for your app to match your K2 token endpoint, such as https://{KUID}.onk2.com/Identity/token/oauth/2. (You can find your KUID by browsing to your onK2 URL and adding **/autodiscover/autodiscover** onto the end of the URL. You can find your KUID in the resulting page.)

 Also, you need to create a secret. Click Certificates & secrets and then click **New client secret**. Once you create the secret, make a note of it as you'll also need to add this to your OAuth Resource.

 Next, configure permissions by clicking **API permissions**. Permissions allow K2 to act on behalf of users. There are **Application** and **Delegated** permissions available in Azure. It's safest to grant both types to the app where specified. Click the **Add a permission** button and find the following Microsoft Graph permissions to add (search usually works best once you click Microsoft Graph):

  + Files.ReadWrite.All
  + Files.ReadWrite.AppFolder
  + Files.ReadWrite.Selected
  + User.Read

  Once you have these permissions granted, you must click the **Grant admin consent** button at the top of the page. This gives your new app the ability to perform OneDrive-related tasks suppported by the connector's methods.

  Lastly, make a note of the endpoints in your environment. At the top of the **Overview** page for your app, click the **Endpoints** button. Here you need to copy the **OAuth 2.0 authorization endpoint (v2)** and the **OAuth 2.0 token endpoint (v2)**.

### Creating the OAuth Resource in K2

  Create your resource that you'll use to configure your service instance. Follow these steps:
  
  1. Browse to K2 Management and expand the **Authentication** node
  2. Expand the **OAuth** node
  3. Click **Resources** and then click **New**
  4. Give your resource a name, select **Microsoft Online** as the Resource Type, and then paste the authorization endpoint (https://login.microsoftonline.com/common/oauth2/v2.0/authorize) into the **Authorization Endpoint** field, the token endpoint (https://login.microsoftonline.com/common/oauth2/v2.0/token) into the **Token Endpoint**, and the token endpoint (https://login.microsoftonline.com/common/oauth2/v2.0/token) into the **Refresh Token Endpoint** 
  5. Add the following parameters to your resource:
  * Resource parameters
    + redirect_uri: your K2 Cloud redirect URI, such as https://kyg4qhn.onk2qa.com/identity/token/oauth/2 
    + client_id: the client ID of your Azure app for all three request values
    + response_type: **Authorization Value** = code
    + grant_type: **Token Value** = authorization_code, **Refresh Value** = refresh_token
    + client_secret: **Token Value** & **Refresh Value** = your client secret
    + scope: https://graph.microsoft.com/Files.Read.All https://graph.microsoft.com/Files.ReadWrite.All https://graph.microsoft.com/Files.ReadWrite.AppFolder https://graph.microsoft.com/Files.ReadWrite.Selected
  6. Save the resource and confirm that it's similar to the following figure

  ![Example OAuth Resource for Microsoft OneDrive](/OAuthResource.png)

  Once you've created your OAuth resource, you can now use it to configure a service instance, but you must first create your service type.

  ### Creating your OneDrive Connector Service Type

  Download the index.js or index.jssp from the repo.

  Once you have your index.jssp file for the OneDrive Connector, create your service type using the example form from the Help topic or one you've built yourself.

  When your service type is created, register a service instance using the OAuth resource you created, and generate SmartObjects.


### License

MIT, found in the [LICENSE](./LICENSE) file.

[www.k2.com](https://www.k2.com)