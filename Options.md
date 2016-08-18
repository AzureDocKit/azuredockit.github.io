---
title: Options
layout: index
---
# Options

The settings are divided in the following sections:

* Azure Workloads
* Document
* SQL Server
* Storage
* Active Directory
* Virtual Machines
* Billing
* Advanced Options

## Azure Workloads

This section has the following settings:

* Data to retrieve : Choose the workloads that you want to include in the documentation

## Document

This section has the following settings:

* Document Template : Choose the template to use to create the document. Five options are available
    * Full : Contains everything that Azure DocKit can generate
    * Executive : Contains high level overview of the environment like billing, overview of the health of your subscription and overview of the changes
    * Changes : Contains all the changes detected since the last document generation
    * Billing : Contains only billing information
    * Custom : Upload a template that you have created

* Generate a Word Document : Check if you need the word document to be generated (Uncheck if you just want to generate a snapshot)

* Generate a global Visio Diagram  : Check if you need the visio documents to be generated (Uncheck if you just want to generate a snapshot)

## SQL Server

This section has the following settings:

* SQL Azure Server List : Enter the credential to use to connect to a SQL Azure Database so that Azure DocKit can generate detailed information about the Databases (like Tables, Stored Procedures...). For each server, you have to enter the following information:
    * Server Name : example *naldefw*
    * Server Login : example *thelogin*
    * Server Password : example *thepasswordoftheloginaccount*


## Storage

This section has the following settings:

* Maximum number of Containers scanned per Storage Account : Azure DocKit will stop scanning Containers after the number specified

* Maximum number of Items scanned per Container : Azure DocKit will stop scanning items (blob) after the number specified

**Changing this settings will affect the document generation time**

## Active Directory

This section has the following settings:

* Maximum number of Users: Azure DocKit will stop scanning users after the number specified

* Maximum number of Changes : Azure DocKit will stop scanning changes after the number specified

**Changing this settings will affect the document generation time**

## Virtual Machines

This section has the following settings:

* Retrieve information inside the virtual machine : Check if you want Azure DocKit to retrieve information from inside the Virtual Machines. Once checked, you can specify the type of information that you need to retrieve from the Virtual Machines.
    * Drives
    * Features
    * Installed Programs
    * Installed Services
    * Startup Programs

## Billing

Azure DocKit supports the following billing types:

* Standard
* EA
* CSP

### Standard

For Standard, you need to enter the following information:

* Offer Id : Type of offer that you are using (click here to see all the codes available : https://azure.microsoft.com/en-us/support/legal/offer-details/)
* Currency code : Enter the currency code (ex : GBP, EUR ...)
* Region code  : Enter the 2 letters code of the region where the offer was bought (ex : GB, DE ...)
* Billing information based on the last X days : Enter the number of days used to retrieve the billing information
* Use this tag to generate a billing report : Enter the tag used to organize your billing
* Apply a ratio when computing prices (%) : Enter the ratio to use. If you enter 110, Azure DocKit will add 10% when generated the graphs

### EA

For EA, you need to enter the following information:
* EA Enrollment Number : When you enroll Azure to your EA you get an Enrollment Number. It’s the enrollment that will be invoiced for the total consumption. In order to find this EA Number, you can log into https://ea.azure.com and you will find it in the upper right corner. The expected format is *51249564*
* EA Billing API Key : This is the API Key require so that Azure DocKit can authenticate to the billing API. To generate that key, you must log into https://ea.azure.com and navigate in the section Usage API AccessKey. The expected format is *ey.......*
* Use this tag to generate a billing report : Enter the tag used to organize your billing
* Apply a ratio when computing prices (%) : Enter the ratio to use. If you enter 110, Azure DocKit will add 10% when generated the graphs

### CSP

For CSP, you need to enter the following information:

* CSP Account Id : Enter your CSP Azure Active Directory Tenant ID
* CSP App Id : Enter the CSP App Id : Click [here](https://msdn.microsoft.com/library/partnercenter/mt709136.aspx) to get more detail on that
* CSP App Key : 
Enter the CSP App Key : Click [here](https://msdn.microsoft.com/library/partnercenter/mt709136.aspx) to get more detail on that
* Use this tag to generate a billing report : Enter the tag used to organize your billing
* Apply a ratio when computing prices (%) : Enter the ratio to use. If you enter 110, Azure DocKit will add 10% when generated the graphs

## Advanced Options

This section has the following sub sections:

* Drop the document in your Azure Subscription and compare documents
* Document Generation Advanced Options
* Email notification 
* Drop the document in your Office 365 tenant  
* Metrics  
* Filters  
* Logging 


### Drop the document in your Azure Subscription and compare documents

This section has the following settings:

* Storage Account Name
     * If you want to store the document in **your** azure environment or if you want to use the **Track Changes** feature, you need to specify a storage that Azure DocKit will use to drop the document once generated and to drop the snapshots for the Track Changes feature.
    * You have to specify the name of the storage (not the full name) : For example, you can specify *myAzureDocKitStorage*
    * **Note that the storage must be an ARM Storage**
    * *CORS Rules will be applied to this storage so we recommend that you create a dedicated storage for that*

*** Please note that this storage account name settings is mandatory if you want to use the Azure DocKit Track Changes feature***

Once specify, click on Test to ensure that the storage can be accessed. If it can, you will then see the two following settings:

* Save Snapshot for future comparison : Check if you want to save a snapshot for the current generation you are about to do. If you don't do that, you will not be able to compare a future document with the current document that you are bout to generate
* Compare to a previous version : Check if you want to include Changes in the document. If you just want to generate a snapshot, you do not need to check that

### Document Generation Advanced Options

This section has the following settings:

* Diagrams resolution : Choose if you want High Resolution or Medium or Low. *Note that it will impact the size of the document that is generated*   
* Embed Visio diagrams : Check if you want to have Embedded Visio diagrams in the document. *Note that it will impact the size of the document that is generated*   
* Generate resource groups diagrams : Check if you want to generate a Visio Diagram for each resource group in your subscription. *Note that it will impact the size of the document that is generated*   
* Generate warnings : Check to include warnings (Billing, Performance, Best Practices & Security)
* Automatically update Table Of Content : Check if you want the Table Of Content to be automatically refresh when you open the document. You will see a dialog box that will ask you to update the table of content.
* Duration (minutes) for access to the generated document : If you don't choose a storage (Office 365 or your own Azure subscription), the document will be securely stored into a Azure DocKit storage. This setting allows you to choose the time allowed to get the document.
* Culture : Specify the culture to be used for diagram generation. This will impact the figures format for example.

### Email notification  

This section has the following settings: 

* Send Notification with links to documents to : Enter the list of emails that should receive a notification when the documents are ready. You can enter multiple emails separated by a space.

* Send Executive Summary to : Enter the list of emails that should receive an executive summary email. The email contains high level information like Billing and Changes . You can enter multiple emails separated by a space.

### Drop the document in your Office 365 tenant   

This section has the following settings: 

* 0ffice 365 Web Site Url : Enter the Url of your site 
* 0ffice 365 Document Library : Enter the Title of the document library 
* 0ffice 365 Login : Enter the Login to connect to your office 365 tenant 
* 0ffice 365 Password : Enter the Login to connect to your office 365 tenant

### Metrics   

This section has the following settings:

* Include metrics diagrams : Check if you want to have metrics diagrams in your documentation. Example of metrics diagram are number of requests for Web Apps and average CPU for Virtual Machines. 
* Generate metrics for the last X days: Specify the number of days to display metrics diagrams

### Filters   

This section has the following settings:

* Resource Groups to explicitly exclude : Enter the resources groups that you DO NOT be included in the document. (Use a space separator to enter multiple)
* Resource Groups to explicitly include : Enter the resources groups that you ONLY want to be included. (Use a space separator to enter multiple)

### Logging 

This section has the following settings: 

*Enable advanced logging (decrease performance) : Activate when you are in troubleshooting mode when in communication with Azure DocKit support team
