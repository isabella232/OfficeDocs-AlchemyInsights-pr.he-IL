---
title: ההתקנה DKIM ב- Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765121"
---
# <a name="setup-dkim-in-office-365"></a>ההתקנה DKIM ב- Office 365

הוראות מלאות עבור קביעת תצורה של DKIM עבור תחומים מותאמים אישית ב- Office 365 הם [כאן](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. עבור **כל** תחום מותאם אישית, עליך ליצור **שתי** רשומות DKIM CNAME בכל לשירות אירוח ה-DNS של התחום שלך (בדרך כלל, רשם תחום). לדוגמה, contoso.com fourthcoffee.com דורשים ארבע רשומות DKIM CNAME: שני עבור contoso.com ומשני עבור fourthcoffee.com.

   רשומות DKIM CNAME עבור **כל** תחום מותאם אישית להשתמש בתבניות הבאות:

   - **שם המחשב המארח**:`selector1._domainkey.<CustomDomain>`

     **נקודות לכתובת או ערך**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **אורך חיים**: 3600

   - **שם המחשב המארח**:`selector2._domainkey.<CustomDomain>`

     **נקודות לכתובת או ערך**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **אורך חיים**: 3600

   \<DomainGUID\> טקסט מימין `.mail.protection.outlook.com` ברשומת MX מותאם אישית עבור התחום המותאם אישית (לדוגמה, `contoso-com` עבור contoso.com תחום). \<InitialDomain\> הוא התחום שבו השתמשת כאשר נרשמת לקבלת Office 365 (לדוגמה, contoso.onmicrosoft.com).

2. לאחר שיצרת את רשומות CNAME לתחומים המותאם אישית שלך, בצע את ההוראות הבאות:

   a. [היכנס ל- Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) באמצעות חשבון בעבודה או בבית ספר השייך לך.

   b. בחר את סמל מפעיל היישומים בפינה הימנית העליונה ובחר באפשרות **ניהול**.

   c. בחלונית הניווט הימנית התחתונה, הרחב **Admin** ובחר **Exchange**.

   d. עבור אל **הגנה** > **DKIM**.

   e. בחר את התחום ולאחר מכן בחר **לזמינה** עבור **הודעות כניסה עבור קבוצת מחשבים זו עם חתימות DKIM**. חזור על שלב זה עבור כל תחום מותאם אישית.
