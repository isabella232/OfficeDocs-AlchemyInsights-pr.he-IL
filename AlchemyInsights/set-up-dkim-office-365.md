---
title: התקנת DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808708"
---
# <a name="setup-dkim"></a>התקנת DKIM

ההוראות המפורטות לקביעת התצורה של DKIM עבור תחומים מותאמים אישית ב-Microsoft 365 נמצאות [כאן](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. עבור **כל** תחום מותאם אישית, עליך ליצור **שתי** רשומות CNAME של DKIM בשירות ה-dns המארח של התחום שלך (בדרך כלל, רשם התחומים). לדוגמה, contoso.com ו-fourthcoffee.com דורשים ארבע רשומות CNAME של DKIM: two עבור contoso.com ושתיים עבור fourthcoffee.com.

   רשומות CNAME של DKIM עבור **כל** תחום מותאם אישית משתמשות בתבניות הבאות:

   - **שם מחשב מארח**: `selector1._domainkey.<CustomDomain>`

     **מצביע על כתובת או ערך**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **שם מחשב מארח**: `selector2._domainkey.<CustomDomain>`

     **מצביע על כתובת או ערך**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> הוא הטקסט שמימין `.mail.protection.outlook.com` לרשומת ה-MX המותאמת אישית עבור התחום המותאם אישית (לדוגמה, `contoso-com` עבור התחום contoso.com). \<InitialDomain\> הוא התחום שבו השתמשת כאשר נרשמת ל-Microsoft 365 (לדוגמה, contoso.onmicrosoft.com).

2. לאחר שיצרת את רשומות CNAME עבור התחומים המותאמים אישית שלך, בצע את ההוראות הבאות:

   מ. [היכנס ל-Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) באמצעות החשבון שלך בעבודה או בבית הספר.

   b. בחר את סמל מפעיל היישומים בפינה הימנית העליונה ובחר באפשרות **ניהול**.

   c. בניווט הימני התחתון, הרחב את **ניהול** ובחר **Exchange**.

   תלת. עבור אל **Protection**  >  **DKIM**Protection.

   e. בחר את התחום ולאחר מכן בחר **הפוך לזמין** עבור **הודעות חתימה עבור תחום זה עם חתימות DKIM**. חזור על שלב זה עבור כל תחום מותאם אישית.
