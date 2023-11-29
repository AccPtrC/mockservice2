## Application Details
|               |
| ------------- |
|**Generation Date and Time**<br>Tue Nov 28 2023 00:33:19 GMT+0000 (Coordinated Universal Time)|
|**App Generator**<br>@sap/generator-fiori-freestyle|
|**App Generator Version**<br>1.11.5|
|**Generation Platform**<br>SAP Business Application Studio|
|**Template Used**<br>simple|
|**Service Type**<br>None|
|**Service URL**<br>N/A
|**Module Name**<br>odatamockservice|
|**Application Title**<br>Mock Service|
|**Namespace**<br>|
|**UI5 Theme**<br>sap_horizon|
|**UI5 Version**<br>1.120.1|
|**Enable Code Assist Libraries**<br>False|
|**Enable TypeScript**<br>False|
|**Add Eslint configuration**<br>False|

## odatamockservice

A Fiori application.

### Starting the generated app

-   This app has been generated using the SAP Fiori tools - App Generator, as part of the SAP Fiori tools suite.  In order to launch the generated app, simply run the following from the generated app root folder:

```
    npm start
```

#### Pre-requisites:

1. Active NodeJS LTS (Long Term Support) version and associated supported NPM version.  (See https://nodejs.org)

#### How to setup a mockservice in SAP BAS by Peter Carandang

1) copy index.html
2) paste in test folder as mockService.html
3) In mockService.html, do the following changes:
-> change src value to "https://sapui5.hana.ondemand.com/1.120.1/resources/sap-ui-core.js" or whichever is the latest version
-> in data-sap-ui-resourceroots, change "./" to "../"
-> in data-sap-ui-oninit, change sap/ui/core/ComponentSupport to the location of your initMockServer file or where it would be
4) Create your localService folder
5) In the local service folder, create your initMockServer.js
6) In the local service folder, add your metadata.xml file
7) In the local service folder, create a mockdata folder
8) In your mockdata folder, create your mock data here as .json file. Name of the .json file is the EntitySet
9) Go to Run Configurations
10) Select Create Configruation
11) For the new Configuration, select the following
-> Filename shouldbe test/mockServer.html
-> Run with mockData should be checked
12) Go to the Terminal (and in the root folder). Type "npm install" and Enter
13) In the run configuration, click the Run button of the created run configuration


