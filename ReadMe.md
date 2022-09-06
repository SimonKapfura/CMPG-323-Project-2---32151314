#  API Project 2 Information
- This is a ReadMe document for Project 2 and it will hold all the information necessary to help the stake holders understand how the project works.
#  Overview
Smart devices such as voice controllers, security lights, smart locks and Wi-Fi-enabled devices can communicate and exchange data over the Internet. Devices form distributed ecosystems that can perform environmental monitoring of homes and buildings. The exposure of IoT device capabilities and data through the Web is fundamental. An IoT Device Management System helps you register, organise, monitor, and remotely manage IoT devices at scale as IoT deployments range in size, complexity, objectives and requirements. An IoT Device Management System keeps track of the whereabouts of all IoT devices deployed by the organisation. Depending on the type of organisation, different categories of devices are used. Each IoT device is initially categorised and registered. Then, IoT devices are deployed throughout the organisation's buildings in predefined zones. Administrators can view all IoT devices, update their properties, add new devices and move them to other zones. Representational State Transfer (REST) is a model and architectural style for web services over HTTP. When this model is used for API design, IoT devices can be managed using the Cloud. Therefore, the IoT Device Management System should be implemented as a set of RESTful APIs. RESTful APIs and services are used as a good practice in the industry to transport data between systems, environments, interfaces and applications. One of the most common use cases is connecting a RESTful API to a data source to manage interaction with the data source. This approach lends many advantages to a solution mostly addressing longevity. RESTful APIs commonly consist of different methods that allow for retrieval of data and manipulation of data (creation, amendment and deletion). As part of this project, you will create a CRUD RESTful API that will connect to a database storing IoT device data. The API should contain at least one get, post, patch and delete method per resource – aligning to the project's requirements. The RESTful API architecture has several endpoints called over HTTP, invoking application code to update a database.
# HTTP Methods:
| HTTP Method           | CRUD operation            | Desctription                                                             |                                 
| :-----                | :---:                     | :----                                                                    |
| GET                   | Read                      | Requests a representation of the specified resource (Mozilla.org, 2022)  |
| POST                  | Create                    | Sends data to the server (Mozilla.org, 2022).                            |
| PATCH                 | Update                    | Applies partial modifications to a resource (Mozilla.org, 2022).         |
| DELETE                | Delete                    |  Deletes the specified resource (Mozilla.org, 2022).                     |
| PUT                   | Update or Replace         | Creates a new resource or replaces an existing one (Mozilla.org, 2022).  |

# Http Responses:
The following information is from Mozilla.org (2022)
| Code Category                               | Status Code                        | Example                  |                                 
| :-----                                      | :---:                              | :----                    |
| Informational responses                     | 100 - 199                          | 100 Continue             |
| Successful responses                        | 200 - 299                          | 200 OK                   |
| Redirection messages                        | 300 - 399                          | 301 Moved Permanently    |
| Client error responses                      | 400 - 499                          | 404 Not Found            |
| Server error responses                      | 500 - 599                          | 503 Service Unavailable  |

# How to use the Connected Office API (Swagger version)
## Get Authorization to use the Service
- Get Authorization by tapping the "Authorize" button on the Swagger UI screen.
- Then Type "Bearer " and add your authentication token and login.
- If the token is valid you should be authirised and can now register account or log in.
## Register or login with Authorization
- After being Authorized you can now create a new account if you are new and login if you already have an account.
- After loging in the system will give you a token to be used again to login with rightful user role.
- Appeon.com (2019), There are two users created at server side (see Add Service Interface and Implementation). 'user1' has admin role, and 'user2' has guest role.
- Admin users and normal users have different permissions.
## Create Zones and Categories to be linked to the devices
- After  loging in,create zones that each devices will be located in.
- The Zone attributes required are zone Id, zone name, zone descreiption and then the date created will be generated automatically by the system.
## Register Devices
- Regitster all the devices in the office to the Device API and add them to  their correct database.
- Each device being registered will require a device ID, a device name, category id to link it to its respective category, zone id to likn it to its respective zone, device status and whether the device is active or not.
- The date field will be automatically added.
## Choose any Http method and execute it
- To view all the data in a specific data set , categories, zones or devices, tap the API method structured like:
-     GET: api/Categories -for all categories
-     GET: api/Zones -for all zones
-     GET: api/Devices for all devices
##  Access specific information with specific ID
- To view a specific item in a specific data set , categories, zones or devices, tap the API method structured like:
-     GET: api/Categories/{id} -for a specific category
-     GET: api/Zones/{id} -for a specific zone
-     GET: api/Devices/{id} -for a specific device
## Add new device, zone or category:
- To add data set , categories, zones or devices, tap the API method structured like:
-     POST: api/Categories -for a specific category
-     POST: api/Zones -for a specific zone
-     POST: api/Devices -for a specific device
## Replace or Update device, zone or category:
- To replace data set , categories, zones or devices, tap the API method structured like:
-     PUT: api/Categories/{id} -for a specific category
-     PUT: api/Zones/{id} -for a specific zone
-     PUT: api/Devices/{id} -for a specific device
## Delete a device, zone or category:
- To delete an item in data set , categories, zones or devices, tap the API method structured like:
-     DELETE: api/Categories/{id} -for a specific category
-     DELETE: api/Zones/{id} -for a specific zone
-     DELETE: api/Devices/{id} -for a specific device
## Update a device, zone or category:
- To update an item in data set , categories, zones or devices, tap the API method structured like:
-     PATCH: api/Categories/{id} -for a specific category
-     PATCH: api/Zones/{id} -for a specific zone
-     PATCH: api/Devices/{id} -for a specific device


# Reference List
- 262588213843476 (2018). Gitignore file to ignore the local appSettings. [online] Gist. Available at: https://gist.github.com/ankitvijay/21b45c70e00846d5ce738005fae0372b [Accessed 3 Sep. 2022].
- Markdownguide.org. (2022). Markdown Cheat Sheet | Markdown Guide. [online] Available at: https://www.markdownguide.org/cheat-sheet/ [Accessed 31 Aug. 2022].
- Atlassian (2022). .gitignore file - ignoring files in Git | Atlassian Git Tutorial. [online] Atlassian. Available at: https://www.atlassian.com/git/tutorials/saving-changes/gitignore [Accessed 3 Sep. 2022].
- bricelam (2021). Connection Strings - EF Core. [online] Microsoft.com. Available at: https://docs.microsoft.com/en-gb/ef/core/miscellaneous/connection-strings [Accessed 3 Sep. 2022].
- mstrand (2016). How to pass multiple parameters to a get method in ASP.NET Core. [online] Stack Overflow. Available at: https://stackoverflow.com/questions/36280947/how-to-pass-multiple-parameters-to-a-get-method-in-asp-net-core [Accessed 4 Sep. 2022].
- Mozilla.org. (2022). HTTP response status codes - HTTP | MDN. [online] Available at: https://developer.mozilla.org/en-US/docs/Web/HTTP/Status#information_responses [Accessed 5 Sep. 2022].
- Appeon.com. (2019). Secure a Web API with a JWT Token. [online] Available at: https://docs.appeon.com/snapdevelop2019/Secure_a_Web_API_with_JWT_Token/index.html [Accessed 5 Sep. 2022].
- Oro Documentation. (2021). Available HTTP Methods - OroCommerce, OroCRM and OroPlatform Documentation. [online] Available at: https://doc.oroinc.com/api/http-methods/#:~:text=The%20primary%20or%20most%20commonly,or%20CRUD)%20operations%2C%20respectively. [Accessed 1 Sep. 2022].
- Mozilla.org. (2022). DELETE - HTTP | MDN. [online] Available at: https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/DELETE [Accessed 2 Sep. 2022].
- Mozilla.org. (2022). PUT - HTTP | MDN. [online] Available at: https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/PUT [Accessed 2 Sep. 2022].
- Mozilla.org. (2022). PATCH - HTTP | MDN. [online] Available at: https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/PATCH [Accessed 2 Sep. 2022].
- Mozilla.org. (2022). POST - HTTP | MDN. [online] Available at: https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/POST [Accessed 2 Sep. 2022].
‌- Mozilla.org. (2022). GET - HTTP | MDN. [online] Available at: https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/GET [Accessed 2 Sep. 2022].
- Jackson, D. (2017). services.AddSwaggerGen() giving error. [online] Stack Overflow. Available at: https://stackoverflow.com/questions/43707733/services-addswaggergen-giving-error [Accessed 5 Sep. 2022].
- domaindrivendev (2021). Swashbuckle.AspNetCore.Cli 6.0.4 does not work for .NET Core 3.1 projects · Issue #2006 · domaindrivendev/Swashbuckle.AspNetCore. [online] GitHub. Available at: https://github.com/domaindrivendev/Swashbuckle.AspNetCore/issues/2006 [Accessed 6 Sep. 2022].
- dotnet (2020). Failed to generate swagger.json with Swashbuckle · Issue #20330 · dotnet/AspNetCore.Docs. [online] GitHub. Available at: https://github.com/dotnet/AspNetCore.Docs/issues/20330 [Accessed 6 Sep. 2022].
- LightToTheEnd (2016). ‘Build failed’ on Database First Scaffold-DbContext. [online] Stack Overflow. Available at: https://stackoverflow.com/questions/38961115/build-failed-on-database-first-scaffold-dbcontext [Accessed 1 Sep. 2022].
- Rick-Anderson (2021). Getting Started - EF Core. [online] Microsoft.com. Available at: https://docs.microsoft.com/en-us/ef/core/get-started/overview/first-app?tabs=netcore-cli [Accessed 2 Sep. 2022].
- Gaander (2018). Azure Web Deploy ‘Publish Failed’. [online] Stack Overflow. Available at: https://stackoverflow.com/questions/51926402/azure-web-deploy-publish-failed [Accessed 4 Sep. 2022].
- VanMSFT (2022). IP firewall rules - Azure SQL Database and Azure Synapse Analytics. [online] Microsoft.com. Available at: https://docs.microsoft.com/en-us/azure/azure-sql/database/firewall-configure?view=azuresql [Accessed 3 Sep. 2022].
- VanMSFT (2022). IP firewall rules - Azure SQL Database and Azure Synapse Analytics. [online] Microsoft.com. Available at: https://docs.microsoft.com/en-us/azure/azure-sql/database/firewall-configure?view=azuresql#create-and-manage-ip-firewall-rules [Accessed 3 Sep. 2022].
- IronAces (2017). EF Code first Keyword not supported: ‘provider’. [online] Stack Overflow. Available at: https://stackoverflow.com/questions/44547572/ef-code-first-keyword-not-supported-provider [Accessed 6 Sep. 2022].
- amiry jd (2022). A named connection string was used, but the name ‘DefaultConnection’ was not found in the application’s configuration. [online] Stack Overflow. Available at: https://stackoverflow.com/questions/70958355/a-named-connection-string-was-used-but-the-name-defaultconnection-was-not-fou [Accessed 3 Sep. 2022].
- Rick-Anderson (2022). Configuration in ASP.NET Core. [online] Microsoft.com. Available at: https://docs.microsoft.com/en-us/aspnet/core/fundamentals/configuration/?view=aspnetcore-6.0 [Accessed 3 Sep. 2022].
- Manan Ghadawala (2020). How JWT Helps in Securing Your API. [online] Appknox.com. Available at: https://www.appknox.com/blog/how-jwt-helps-in-securing-your-api [Accessed 2 Sep. 2022].

‌

‌

‌

‌
‌

‌

‌

‌

‌

‌
‌
‌
‌

‌

‌
‌
