---
title: הגדרת DKIM
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
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108557"
---
# <a name="setup-dkim"></a>הגדרת DKIM

ההוראות המלאות לקביעת התצורה של DKIM עבור תחומים מותאמים אישית ב- Microsoft 365 [נמצאות כאן](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. עבור **כל** תחום מותאם אישית, עליך ליצור **שתי** רשומות DKIM CNAME בשירות אירוח ה- DNS של התחום שלך (בדרך כלל, רשם התחומים). לדוגמה, contoso.com ו- fourthcoffee.com דורשים ארבע רשומות DKIM CNAME: שתיים עבור contoso.com ו- 2 עבור fourthcoffee.com.

   רשומות CNAME של DKIM עבור כל **תחום** מותאם אישית משתמשות בתבניות הבאות:

   - **שם מארח**: `selector1._domainkey.<CustomDomain>`

     **מצביע לכתובת או לערך**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **שם מארח**: `selector2._domainkey.<CustomDomain>`

     **מצביע לכתובת או לערך**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> הוא הטקסט מימין ברשומת ה- MX המותאמת אישית עבור `.mail.protection.outlook.com` התחום המותאם אישית (לדוגמה, `contoso-com` עבור contoso.com). \<InitialDomain\>הוא התחום שהשתמשת בו כאשר נרשמת Microsoft 365 (לדוגמה, contoso.onmicrosoft.com).

2. לאחר יצירת רשומות CNAME עבור התחומים המותאמים אישית שלך, בצע את ההוראות הבאות:

   a. [היכנס כדי Microsoft 365 באמצעות](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) החשבון שלך בעבודה או בבית הספר.

   b. בחר את סמל מפעיל היישומים בפינה הימנית העליונה ובחר באפשרות **ניהול**.

   c. בניווט הימני התחתון, הרחב את **מנהל** מערכת ובחר **Exchange**.

   d. עבור אל **הגנה**  >  **DKIM**.

   e. בחר את התחום ולאחר מכן בחר **הפוך לזמין** **עבור חתום על הודעות עבור תחום זה עם חתימות DKIM**. חזור על שלב זה עבור כל תחום מותאם אישית.
