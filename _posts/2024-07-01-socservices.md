---
title: My experience of transforming a niche Android app into a product that is used by sevral large cities and communities
date: 2024-07-01 12:00:00 -500
categories: [Android, Personal]
tags: [Android, Mifare, RFID, MifareClassic, SmartCard]
---
![socservices-power-of-android](/assets/images/socservices-power-of-android.png)

![socservices-from-proto-to-prod](/assets/images/socservices-from-proto-to-prod.png)

In this post, I would like to share my experience of transforming a niche Android app into a product that is used by sevral large cities and communities. The app's client base was significantly expanded due to a thorough comprehension of Android features and clear app architecture. 

The "Non-Financial Processing: Social Services" Android app was one of the first apps I worked on at the Financial Services Agency.

The initial version of this software was developed exclusively for a single medical organization. It was used to find services assigned to patients and monitor its provision. This medical organization intended to utilize it on stationary point-of-sale terminals. The patient's bank card number was read with a pin-pad and used as an identifier.

The further expansion of the app's client base encountered resistance. The reason was that new clients were primarily interested in using this application for ground staff - social and medical workers who visit and help customers at home.

However, the application was not fully meeting the needs of such clients due to the following reasons.

❌ It required an expensive and heavy POS terminal with pin-pad, and agreement with a bank.

❌ Some ground staff worked in mountains with poor internet coverage, but app required internet connection to provide information.

❌ Several recipients of social services expressed dissatisfaction with the utilization of their bank card as a means of identification for free of charge social services.

Having a comprehensive understanding of Android capabilities allowed me to propose and develop the 2.0 version of a software that eradicated all shortcomings.

🛠 Clear architecture and compliance with SOLID principles allowed quick and easy porting of software from POS-terminal OS to Android OS. 

✅ This allowed clients to replace bulky $650 POS terminal and pin-pad with $50 smartphone.

🛠 My knowledge of android.nfc.tech allowed me to implement a custom bank card reader feature on regular smartphones with NFC.

✅ This eliminated the need for an external pin-pad.

🛠 App had multi modular architecture. Each Gradle module was fully independent feature. 

✅ This allowed us to quickly build new app variations and easily meet the individual business flows of each new client.

🛠 My deep knowledge of android.nfc.tech allowed me to design a custom Smart Social Card based on Mifare. This new card was designed with similar principles to smart cards for public transportation. The Smart Social Card contained details regarding services, and the Android application functioned as a validator. 

✅ This allowed users to use both bank card and the Mifare card without a constant internet connection.

The new version of software was a great success as it spread to entire cities and communities.

This demonstrates that a clear app architecture and a deep understanding of the software platform are useful not only for development, but also for expanding a business application of a product.