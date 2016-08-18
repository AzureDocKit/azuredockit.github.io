---
title: Troubleshooting
layout: index
---
# Troubleshooting

**Before starting any troubleshooting, you need to logout from the Azure management portals (https://manage.windowsazure.com and https://portal.azure.com) and go back to Azure DocKit in private mode. Indeed, most of the issues are due to the fact that wrong credentials are used when trying to Sign In into Azure DocKit.**

* **When I Sign In into Azure DocKit, the list of subscriptions is emtpy.**
  * If you do not see any subscription in the drop down list, it means that you do not have access to any subscription. To ensure that you have access to at least one subscription, you can connect to https://manage.windowsazure.com and https://portal.azure.com. If you do not see any subscription in those 2 portals it means that you have not the required access.

* **When I Sign In into Azure DocKit, I get an error message saying Calling principal cannot consent due to lack of permissions.**
  * You must have checked the checkbox specifying that you are an Azure Active Directory Global Admin. This requires that you are Azure AD Global Admin which is not the case. Restart the process without checking the checkbox.

* **I have a G2-U license but the user that is licensed do not have appropriate permissions on the subscription that I need to document. I need to use another account.**
  * Azure DocKit supports this scenario.
  * The first step is to Sign In into Azure DocKit using the account that is licensed (even if this account has not privileges on the subscription to document).
  * Once Logged In, you will see a button on the top of the windows that allows you to change user. Click on that and then you need to enter the account that you want to use.
  * Once done, click on Log Out.
  * Now, go back to the Azure DocKit home page and Sign In with this account.
  * You should now have a valid license.
  * *Note that you have 5 minutes to do that*
  * ** Note that it is not legal to use this mechanism to give a license to someone else**

* **I have a G2-T license but the user that is licensed do not have appropriate permissions on the subscription that I need to document. I need to use another account.**
  * Azure DocKit supports this scenario.
  * The first step is to Sign In into Azure DocKit using the account that is licensed (even if this account has not privileges on the subscription to document).
  * Once Logged In, you will see a button on the top of the windows that allows you to change user. Click on that and then you need to enter the account that you want to use.
  * Once done, click on Log Out.
  * Now, go back to the Azure DocKit home page and Sign In with this account.
  * You should now have a valid license.
  * *Note that you have 5 minutes to do that*
  * ** Note that it is not legal to use this mechanism to give a license to someone else**

* **The first question being asked is the tenant name. What should I enter in this.**
  * Have a look at http://www.azuredockit.com/2016/05/19/what-tenant-should-i-use-to-generate-documentation-using-azure-dockit/
  * It will give you all the details on how to find which tenant to use
