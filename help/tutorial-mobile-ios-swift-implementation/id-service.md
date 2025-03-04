---
title: Add the Adobe Experience Platform Identity Service with tags
description: Learn how to add the Adobe Experience Platform Identity Service extension and use the Set Customer IDs action to collect customer ids. This lesson is part of the Implement the Experience Cloud in Mobile iOS Swift Applications tutorial.
solution: Experience Platform, Data Collection, Experience Cloud Services
exl-id: 0e871120-7ec0-44cc-bf58-f5c79b69b463
---
# Add the Adobe Experience Platform Identity Service

The [Adobe Experience Platform Identity Service](https://experienceleague.adobe.com/docs/id-service/using/home.html) sets a common visitor id across all Adobe solutions in order to power Experience Cloud capabilities such as audience-sharing between solutions. You can also send your own customer ids to the Service to enable cross-device targeting and integrations with your Customer Relationship Management (CRM) system.

The Identity Service is part of the Mobile Core extension, ***so you have already implemented it when you installed the Mobile SDK***! At present time, this tutorial does not include instructions for setting Customer Ids. Please see the documentation for details on [how to set Customer Ids](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/mobile-core/identity/identity-api-reference).

## Validation Steps

To validate the calls to the Identity Service, run the sample app in Xcode or Developer Studio, open the Debug Console and look for the request and the response:

1. **Request to the Identity Service** (filter your console to `demdex.net`) In this example, the ID (`d_mid`) has already been set and is just being reported up again)

    ```swift
    2019-01-15 12:11:45.164590-0500 BusDemoSwift[52399:5056322] [AMSDK DEBUG <com.adobe.module.identity>]: Sending request (https://dpm.demdex.net/id?d_rtbd=json&d_ver=2&d_orgid=7ABB3E6A5A7491460A495D61@AdobeOrg&d_mid=17179986463578698626041670574784107777&d_blob=j8Odv6LonN4r3an7LhD3WZrU1bUpAkFkkiY1ncBR96t2PTI&dcs_region=9)
    ```

1. **Response from the Identity Service** (filter your console to `ID Service`). Note how the `mid` value matches the `d_mid` value in the request above:

    ```swift
    2019-01-15 12:11:45.681821-0500 BusDemoSwift[52399:5056322] [AMSDK DEBUG <com.adobe.module.identity>]: ID Service - Got ID Response (mid: 17179986463578698626041670574784107777, blob: j8Odv6LonN4r3an7LhD3WZrU1bUpAkFkkiY1ncBR96t2PTI, hint: 9, ttl: "604800000 ms")
    ```

[Next "Add Adobe Target Support" >](target.md)
