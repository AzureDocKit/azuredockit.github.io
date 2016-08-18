---
title: Which Tenant To Use
layout: index
---
# Azure Active Directory Tenant to use to Sign In in Azure DocKit

When you navigate to the Azure DocKit generation portal, you will be first asked to enter the Name of the Tenant.

If you have access to an Azure Subscription with a Microsoft Account or with an Azure AD Account, it means that **there is an Azure AD** attached to the subscription.
In Azure, when you connect to the management portal, you can see multiple Azure Active Directories that are all the Directories you have access to:

![HomePage](http://azuredockitwebsite.azurewebsites.net/wp-content/uploads/2016/08/ADKNewLookTenant.png)

Even if your account is in multiple Active Directory, it is mandatory that you use the Active Directory that is associated to the subscription that you want to document. Note that there is **only one** Active directory that is associated to the subscription.
In order to find the directory, you can click on the settings menu and you will find the directory to use in the Directory column:

![Azure AD](http://azuredockitwebsite.azurewebsites.net/wp-content/uploads/2016/05/051916_1523_Whattenants2.png)

You can now go back to https://generate.azuredockit.com and specify this tenant.


If you don’t have access to the old portal, you can connect to the new one (https://portal.azure.com) and then enter the old portal address (https://manage.windowsazure.com) and you will see that the tenant name is specified in the error window :

![Find Tenant Name](http://azuredockitwebsite.azurewebsites.net/wp-content/uploads/2016/05/ADK_AADTEnantNewPortal.png)
