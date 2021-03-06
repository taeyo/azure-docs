---
title: Create, link, delete, or move an integration account in Azure logic apps | Microsoft Docs
description: How to create an integration account, and link it to your logic apps
services: logic-apps
documentationcenter: .net,nodejs,java
author: divyaswarnkar
manager: anneta
editor: 

ms.assetid: d3ad9e99-a9ee-477b-81bf-0881e11e632f
ms.service: logic-apps
ms.workload: integration
ms.tgt_pltfrm: na
ms.devlang: na
ms.topic: article
ms.date: 02/23/2017
ms.author: LADocs; divswa

---

# What is an integration account?

An integration account provides a way for your enterprise integration apps, 
specifically logic apps, to access and manage B2B artifacts, 
for example, trading partners, agreements, maps, schemas, certificates, and so on. 
To provide this access, link your integration account to your logic app, 
after making sure that both the integration account and logic app 
have the *same Azure location*.

## Create an integration account

1. Sign in to the [Azure portal](http://portal.azure.com "Azure portal"). 

2. From the main Azure menu, select **All services**. 
In the search box, enter "integration", 
and then select **Integration accounts**.

   ![Create integration account](./media/logic-apps-enterprise-integration-accounts/account-1.png)

3. At the top of the page, choose **Add**.

   ![Choose Add](./media/logic-apps-enterprise-integration-accounts/account-3.png)

4. Name your integration account and select the Azure subscription that you want to use. 
You can either create a new **Resource group** or select an existing resource group. 
Select a **Location** to host your integration account and a **Pricing Tier**. 
When you're ready, choose **Create**.

   ![Provide details for your integration account](./media/logic-apps-enterprise-integration-accounts/account-4.png)

   Azure provisions your integration account 
   in the selected location, which should complete within one minute.

5. Refresh the page. You see your new integration account listed.

   ![Your new integration account appears](./media/logic-apps-enterprise-integration-accounts/account-5.png) 

Next, link the integration account that you created to your logic app. 

## Link an integration account to a logic app

To give your logic apps access to B2B artifacts, such as trading partners, 
agreements, maps, and schemas in your integration account, 
link the integration account to your logic app. 

1. In the Azure portal, select your logic app, and check your logic app's location.

   ![Select your logic app, check location](./media/logic-apps-enterprise-integration-accounts/linkaccount-1.png)

2. Under **Settings**, select **Integration Account**.

   ![Select "Integration Account"](./media/logic-apps-enterprise-integration-accounts/linkaccount-2.png)

3. From the **Select an Integration account** list, 
select the integration account you want to link to your logic app. 
To finish linking, choose **Save**.

   ![Select your integration account](./media/logic-apps-enterprise-integration-accounts/linkaccount-3.png)

   You get a notification that shows your integration account is linked to your logic app, 
   and that all artifacts in your integration account are now available to your logic app.

   ![Your logic app is linked to your integration account](./media/logic-apps-enterprise-integration-accounts/linkaccount-5.png)

Now that your integration account is linked to your logic app, 
you can use the B2B connectors in your logic app. 
Some common B2B connectors include XML validation and flat file encode/decode.  

## Delete your integration account

1. From the main Azure menu, select **All services**. 
In the search box, enter "integration", 
and then select **Integration accounts**.

   ![Find your integration account](./media/logic-apps-enterprise-integration-accounts/account-1.png)

2. Select the integration account that you want to delete.

	![Select integration account to delete](./media/logic-apps-enterprise-integration-accounts/account-5.png)

3. On the menu, choose **Delete**.

	![Choose "Delete"](./media/logic-apps-enterprise-integration-accounts/delete.png)

4. Confirm your choice to delete the integration account.

## Move your integration account

To move an integration account to another Azure subscription or resource group, 
follow these steps. After you move the integration account, 
make sure that you update all scripts to use the new resource IDs.

1. From the main Azure menu, select **All services**. 
In the search box, enter "integration", 
and then select **Integration accounts**.

   ![Find your integration account](./media/logic-apps-enterprise-integration-accounts/account-1.png)

2. Select the integration account that you want to move. 
Under **Settings**, choose **Properties**.

   ![Select integration account to move. Under Settings, choose Properties](./media/logic-apps-enterprise-integration-accounts/move.png)

3. Change the resource group or Azure subscription that's associated with your integration account.

   ![Choose Change resource group or Change subscription](./media/logic-apps-enterprise-integration-accounts/move-2.png)

## Next steps

* [Learn more about agreements](../logic-apps/logic-apps-enterprise-integration-agreements.md "Learn about enterprise integration agreements")  

