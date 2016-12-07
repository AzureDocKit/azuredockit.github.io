---
title: Create Azure Documentation with your own template
layout: index
---

# Create Azure Documentation with your own template

Azure DocKit gives you the ability to generate detailed documentation of everything you have in your Azure Subscription. The generated document gives you plenty of information and also rich Visio Diagrams. Would it be nice if you could control the output document that is generated for you? Change your logo, add text, remove sections, change colors…. You can do all that. Let’s see how.

First step is to get the template document. You can download it from [here](https://generate.azuredockit.com/templates/AzureTemplate_Full.docx)

Once you have open the document, you need to ensure that you can see the Developer Tab:
![Developer Tab](http://azuredockitwebsite.azurewebsites.net/wp-content/uploads/2016/03/032216_1514_CreateAzure1.png)
 
By using this tab, you will be able to switch the document in Design Mode which will display all the Content Controls that are in the document:
![Content Controls](http://azuredockitwebsite.azurewebsites.net/wp-content/uploads/2016/03/032216_1514_CreateAzure2.png)
 
As you can see in the Executive Summary section, the document is built with many Content Controls that are dynamically filled by Azure DocKit when it generates the documentation.
If you want to change the template, you can do as follow:
**Change the look and feel of the document**

As the template is a word document, the best way to change the look and feel of the document is to edit the Heading styles. In order to do that, right click on the Heading and click on modify:
![Change Headings](http://azuredockitwebsite.azurewebsites.net/wp-content/uploads/2016/03/032216_1514_CreateAzure3.png)

Then, you can change the color or styles as you want.
You can also change the First Page of the document. For instance, you can change the colors and the logo:

![First Page](http://azuredockitwebsite.azurewebsites.net/wp-content/uploads/2016/03/032216_1514_CreateAzure4.png)
 
**Remove content**

If you don’t need a specific section or content in a section, you can just remove it.
For instance, if you don’t need the Web Site Diagnostics section, you can use the navigation Pane and delete it:
![Delete Content](http://azuredockitwebsite.azurewebsites.net/wp-content/uploads/2016/03/032216_1514_CreateAzure5.png)
 
 
If in this specific section, you want to remove only a specific line in the table, you can also do that.
 
*Add content*

You can also add content in the document. For example, if you don’t like the boilerplate text that is used in the document, you can edit it:
 
![Add Content](http://azuredockitwebsite.azurewebsites.net/wp-content/uploads/2016/03/032216_1514_CreateAzure7.png)
 
The last step before saving the update Template is to update the Table of Content. You **must** go on the Table of Content and right click and select update:

![Update TOC](http://azuredockitwebsite.azurewebsites.net/wp-content/uploads/2016/03/032216_1514_CreateAzure8.png)
 
This step is really mandatory as Azure DocKit is using Table of Content to remove empty section. So if you don’t’ do that, you may have a corrupted document.
Also, note that you cannot change the Table of Content like not displaying all the Heading levels otherwise it will corrupt the document.
Use the template

Now that you have made the hard work, it’s time to use the template to generate a new document. To do that, click on the settings button of the Azure DocKit Portal and go to the template tab. Click on browse and then select your template:

![Use Template](http://azuredockitwebsite.azurewebsites.net/wp-content/uploads/2016/03/032216_1514_CreateAzure9.png)
 

Then click Generate!
***Warnings***

**
Changing the Template can result in a generated document that is corrupted, so please ensure you read this: 
* Always update the Table of Content before saving the document 
* Proceed to small changes and try to generate the document and do other changes to ensure that you haven’t made any change that corrupt the document 
* Do not modify the structure of the document (like removing Content Control that are Placeholders) 
* Once you have changed the template, you will not get the new template stuffs so our advice is to keep the personalization minimal so that you can easily redo it if we provide a new template. 
**

