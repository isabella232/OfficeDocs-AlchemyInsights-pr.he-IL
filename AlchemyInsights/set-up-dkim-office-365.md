---
title: הגדרת DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509385"
---
# <a name="setup-dkim"></a>הגדרת DKIM

ההנחיות השלמות לקביעת התצורה של DKIM עבור תחומים מותאמים אישית ב-Microsoft 365 נמצאים [כאן](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. עבור **כל** תחום מותאם אישית, עליך ליצור **שתי** רשומות של dkim CNAME בשירות ה-DNS המארח של התחום שלך (בדרך כלל, רשם התחום). לדוגמה, contoso.com ו-fourthcoffee.com דורשות ארבע רשומות של DKIM CNAME: שתיים עבור contoso.com ושתיים עבור fourthcoffee.com.

   רשומות ה-DKIM CNAME עבור **כל** תחום מותאם אישית משתמשות בתבניות הבאות:

   - **שם מחשב מארח**:`selector1._domainkey.<CustomDomain>`

     **נקודות לכתובת או לערך**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **שם מחשב מארח**:`selector2._domainkey.<CustomDomain>`

     **נקודות לכתובת או לערך**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\>הוא הטקסט שמשמאל `.mail.protection.outlook.com` לרשומת ה-MX המותאמת אישית עבור התחום המותאם אישית (לדוגמה, `contoso-com` עבור התחום contoso.com). \<InitialDomain\>הוא התחום בו השתמשת כאשר נרשמת עבור Microsoft 365 (לדוגמה, contoso.onmicrosoft.com).

2. לאחר שיצרת את רשומות ה-CNAME עבור התחומים המותאמים אישית שלך, השלם את ההוראות הבאות:

   קצת. [היכנס ל-Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) עם העבודה שלך או חשבון בית הספר.

   b. בחר את סמל מפעיל היישומים בפינה הימנית העליונה ובחר באפשרות **ניהול**.

   c. בניווט השמאלי התחתון, הרחב את **Admin** ובחר באפשרות **Exchange**.

   d. . לך **להגנה**  >  **DKIM**.

   e. בחר את התחום ולאחר מכן בחר **באפשרות ' הפעל** **הודעות ' עבור תחום זה עם חתימות dkim**. חזור על שלב זה עבור כל תחום מותאם אישית.
