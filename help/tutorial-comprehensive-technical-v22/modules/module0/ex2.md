---
title: Getting Started - Create your Datastream
description: Getting Started - Create your Datastream
kt: 5342
audience: Data Engineer, Data Architect
doc-type: tutorial
activity: develop
exl-id: 146e9e4e-2726-46e2-a6ca-62c4ce6f8ba1
---

# 0.2 Create your Datastream

Go to [https://experience.adobe.com/#/data-collection/](https://experience.adobe.com/#/data-collection/). After the previous exercise, you now have two Data Collection properties: one for web and one for mobile.

![DSN](./images/launchprop.png)

These properties are almost ready to be used, but before you can start collecting data using these properties you need to set up a datastream. You'll get more information around the concept of what a datastream is and what it means in Exercise 1.2.

For now, please follow these steps.

## 0.2 Create your Datastream for Web

Click **[!UICONTROL Datastreams]**.

![Click Edge Configuration icon in the left navigation](./images/edgeconfig1a.png)

Click **[!UICONTROL New Datastream]**.

![Click Edge Configuration icon in the left navigation](./images/edgeconfig1.png)

For the **[!UICONTROL Friendly Name]**, and for the optional description, enter `--demoProfileLdap--` - Demo System Datastream and click **Save**.

![Name the Edge Configuration and save](./images/edgeconfig2.png)

You'll then see this:

![Name the Edge Configuration and save](./images/edgeconfig3.png)

Toggle on **[!UICONTROL Adobe Experience Platform]** which will expose additional fields. You'll then see this:

![Name the Edge Configuration and save](./images/edgeconfig4.png)

For **[!UICONTROL Sandbox]**, select your sandbox name, which should be `--aepSandboxId--`.

![Name the Edge Configuration and save](./images/edgeconfig5.png)

For Event Dataset, select **Demo System - Event Dataset for Website (Global v1.1)** and for Profile Dataset, select **Demo System - Profile Dataset for Website (Global v1.1)**.

![Name the Edge Configuration and save](./images/edgeconfig7.png)

That's it for now. In [Module 1](./../module1/data-ingestion-launch-web-sdk.md) you'll learn more about Web SDK and how to configure all of its capabilities.

You now have this. Click **Save**.

![Name the Edge Configuration and save](./images/edgeconfig8.png)

You'll then see that your datastream consists of 3 environments.

![Name the Edge Configuration and save](./images/edgeconfig9.png)

In the left menu, clik **[!UICONTROL Tags]**.

Filter the search results to see your two Data Collection properties. Open the property for **Web** by clicking it.

![Name the Edge Configuration and save](./images/edgeconfig10a.png)

You'll then see this. Click **Extensions**.

![Name the Edge Configuration and save](./images/edgeconfig11.png)

On the Adobe Experience Platform Web SDK extension, click **Configure**.

![Name the Edge Configuration and save](./images/edgeconfig12.png)

You'll then see this. For **Datastreams**, you'll currently see a dummy value set to 1. You now need to click the **Choose from list** radio-button. In the dropdown list, select the Datastream you created earlier.

![Name the Edge Configuration and save](./images/edgeconfig13.png)

Make sure to have selected your **Datastream**. TIP: You can filter the results in the dropdown easily by typing your `--demoProfileLdap--`.

![Name the Edge Configuration and save](./images/edgeconfig14.png)

Scroll down until you see **Data Collection**. Please ensure that the checkbox for **Enable click data collection** is not enabled. Click **Save** to save your changes.

![Name the Edge Configuration and save](./images/edgeconfig14a.png)

Go to **Publishing Flow**.

![Name the Edge Configuration and save](./images/edgeconfig15.png)

Click the **...** for **Main**, then click **Edit**.

![Name the Edge Configuration and save](./images/edgeconfig16.png)

Click **Add All Changed Resources** and then click **Save & Build for Development**.

![Name the Edge Configuration and save](./images/edgeconfig17.png)

Your changes are now being published and will be ready in a couple of minutes.

## 0.2 Create your Datastream for Mobile

Go to [https://experience.adobe.com/#/data-collection/](https://experience.adobe.com/#/data-collection/). 

Open the dropdown menu and click **[!UICONTROL Datastream]**.

![Click Datastream icon in the left navigation](./images/edgeconfig1a.png)

Click **[!UICONTROL New Datastream]**.

![Click Datastream icon in the left navigation](./images/edgeconfig1.png)

For the **[!UICONTROL Friendly Name]**, and for the optional description, enter `--demoProfileLdap--` - Demo System Datastream (Mobile).
Click **[!UICONTROL Save]**.

![Name the Datastream and save](./images/edgeconfig2m.png)

You'll then see this:

![Name the Datastream and save](./images/edgeconfig3m.png)

Toggle on **[!UICONTROL Adobe Experience Platform]** which will expose additional fields. You'll then see this:

![Name the Datastream Configuration and save](./images/edgeconfig4m.png)

For **[!UICONTROL Sandbox]**, select your sandbox name.

![Name the Datastream Configuration and save](./images/edgeconfig5m.png)

For Event Dataset, select **Demo System - Event Dataset for Mobile App (Global v1.1)** and for Profile Dataset, select **Demo System - Profile Dataset for Mobile App (Global v1.1)**. Click **Save**.

![Name the Datastream Configuration and save](./images/edgeconfig7m.png)

You'll then see that your Datastream consists of 3 environments.

![Name the Datastream Configuration and save](./images/edgeconfig9m.png)

Your Datastream is now ready to be used in your Adobe Experience Platform Data Collection Client property for Mobile.

Go to **Tags** and filter the search results to see your two Data Collection properties. Open the property for **Mobile** by clicking it. 

![Name the Edge Configuration and save](./images/edgeconfig10am.png)

You'll then see this. Click **Extensions**.

![Name the Edge Configuration and save](./images/edgeconfig11m.png)

On the **Adobe Experience Platform Edge Network** extension, click **Configure**.

![Name the Edge Configuration and save](./images/edgeconfig12m.png)

You'll then see this. For the **Datastreams**, you'll currently see a dummy value set to 1. You now need to click the **Choose from list** radio-button. In the dropdown list, select the Datastream you created earlier. Click **Save** to save your changes.

![Name the Edge Configuration and save](./images/edgeconfig13m.png)

Go to **Publishing Flow**.

![Name the Edge Configuration and save](./images/edgeconfig15m.png)

Click the **...** next to **Main**, then click **Edit**.

![Name the Edge Configuration and save](./images/edgeconfig16m.png)

Click **Add All Changed Resources**, then click **Save & Build for Development**.

![Name the Edge Configuration and save](./images/edgeconfig17m.png)

Your changes are now being published and will be ready in a couple of minutes.

Next Step: [0.3 Create your Enablement Configuration ID](./ex3.md)

[Go Back to Module 0](./getting-started.md)

[Go Back to All Modules](./../../overview.md)