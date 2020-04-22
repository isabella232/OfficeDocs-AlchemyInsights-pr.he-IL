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
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645673"
---
# <a name="setup-dkim"></a>הגדרת DKIM

ההנחיות השלמות לקביעת התצורה של DKIM עבור תחומים מותאמים אישית ב-Microsoft 365 נמצאים [כאן](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. עבור **כל** תחום מותאם אישית, עליך ליצור **שתי** רשומות של dkim CNAME בשירות ה-DNS המארח של התחום שלך (בדרך כלל, רשם התחום). לדוגמה, contoso.com ו-fourthcoffee.com דורשות ארבע רשומות של DKIM CNAME: שתיים עבור contoso.com ושתיים עבור fourthcoffee.com.

   רשומות ה-DKIM CNAME עבור **כל** תחום מותאם אישית משתמשות בתבניות הבאות:

   - **שם מחשב מארח**:`selector1._domainkey.<CustomDomain>`

     **נקודות לכתובת או לערך**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **שם מחשב מארח**:`selector2._domainkey.<CustomDomain>`

     **נקודות לכתובת או לערך**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> הוא הטקסט שמשמאל `.mail.protection.outlook.com` לרשומת ה-MX המותאמת אישית עבור קבוצת המחשבים המותאמת אישית `contoso-com` (לדוגמה, עבור קבוצת המחשבים contoso.com). \<אתחאלתחום\> הוא התחום שבו השתמשת כאשר נרשמת ל365 של Microsoft (לדוגמה, contoso.onmicrosoft.com).

2. לאחר שיצרת את רשומות ה-CNAME עבור התחומים המותאמים אישית שלך, השלם את ההוראות הבאות:

   קצת. [היכנס ל-Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) עם העבודה שלך או חשבון בית הספר.

   b. בחר את סמל מפעיל היישומים בפינה הימנית העליונה ובחר באפשרות **ניהול**.

   c. בניווט השמאלי התחתון, הרחב את **Admin** ובחר באפשרות **Exchange**.

   d. . לך **להגנה** > **.**

   e. בחר את התחום ולאחר מכן בחר **באפשרות ' הפעל** **הודעות ' עבור תחום זה עם חתימות dkim**. חזור על שלב זה עבור כל תחום מותאם אישית.
