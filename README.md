simple-viewer-template
==========================

Simple Viewer is a configurable application template that provides a simple and easy to use framework for viewing web maps in browsers or devices.

[View it live](http://www.arcgis.com/apps/SimpleViewer/index.html?webmap=6c4e81f90c4b4935945e9b623c5247e0)


#July 2015 Release Updates
-  **Custom URL Parameters:** The template now supports the ability to define a custom url parameter along with the search layer and field. This can be used to build applications that display a particular feature at application startup. For example if your app displays parcel features you could define a custom url parameter called parcel and then users can navigate there directly by appending ?parcel=1245243242343 and the map will zoom to that feature on startup. Define these values using by setting the customUrlParam and customUrlLayer properties in config/defaults.js. 

#Features
**Simple Map Viewer** is a configurable application template that provides a simple user experience for exploring any web map. It has been designed to support a variety of form factors - browsers, phones, and tablets. The template can be configured with the following options: 

- **Map:** Choose the web map used in your application. 
- **Title Text:** The application title. The default title is the web map name.
- **Search:** Displays the search box to enable navigation to addresses and places. 
- **About** Displays the web map description or custom content defined in the application configuration in an About panel. 

Simple Map Viewer can be accessed via the ArcGIS template gallery or item details. The application source code can be downloaded for further customization and published from your own web server.

## Instructions

1. Download and unzip the .zip file or clone the repository.
2. Web-enable the directory.
3. Access the .html page.
4. Start writing your template!

[New to Github? Get started here.](https://github.com/)

## Deploying

1. To deploy this application, download the template from Portal/ArcGIS Online and unzip it.
2. Copy the unzipped folder containing the web app template files, such as index.html, to your web server. You can rename the folder to change the URL through which users will access the application. By default the URL to the app will be `http://<Your Web Server>/<app folder name>/index.html`
3. Change the sharing host, found in defaults.js inside the config folder for the application, to the sharing URL for ArcGIS Online or Portal. For ArcGIS Online users, keep the default value of www.arcgis.com or specify the name of your organization.
  - ArcGIS Online Example:  `"sharinghost": location.protocol + "//" + ???<your organization name>.maps.arcgis.com`
  - Portal Example where `arcgis` is the name of the Web Adaptor: `"sharinghost": location.protocol + "//" + "webadaptor.domain.com/arcgis"`
4. If you are using Portal or a local install of the ArcGIS API for JavaScript, change all references to the ArcGIS API for JavaScript in index.html to refer to your local copy of the API. Search for the references containing `"//js.arcgis.com/3.13"` and replace this portion of the reference with the url to your local install.
  - For example: `"//webadaptor.domain.com/arcgis/jsapi/jsapi"` where `arcgis` is the name of your Web Adaptor.
5. Copy a map or group ID from Portal/ArcGIS Online and replace the default web map ID in the application???s default.js file. You can now run the application on your web server or customize the application further.

 **Note:** If your application edits features in a feature service, contains secure services or web maps that aren't shared publicly, or generate requests that exceed 200 characters, you may need to set up and use a proxy page. Common situations where you may exceed the URL length are using complex polygons as input to a task or specifying a spatial reference using well-known text (WKT). For details on installing and configuring a proxy page see [Using the proxy](https://developers.arcgis.com/javascript/jshelp/ags_proxy.html). If you do not have an Internet connection, you will need to access and deploy the ArcGIS API for JavaScript documentation from [developers.arcgis.com](https://developers.arcgis.com/).


#Requirements

- Notepad or HTML editor
- Some background with HTML, CSS and JavaScript
- Experience with the ArcGIS API for JavaScript is helpful. 

#Resources

- [ArcGIS API for JavaScript Resource Center](http://help.arcgis.com/en/webapi/javascript/arcgis/index.html)
- [ArcGIS Online] (http://www.arcgis.com)
- Want to create your own template? View the [Application Boilerplate](https://github.com/Esri/application-boilerplate-js) to get started. 
- [View the Simple Map Viewer template on ArcGIS Online](http://www.arcgis.com/home/item.html?id=9ae78842d98a4178bd4a794449324349)

#Issues
Found a bug or want to request a new feature? Please let us know by submitting an issue. 

#Contributing
Anyone and everyone is welcome to contribute. 

#Licensing 

Copyright 2012 Esri

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.

A copy of the license is available in the repository's license.txt file.

