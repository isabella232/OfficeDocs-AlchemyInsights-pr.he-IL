---
title: הגדרת DKIM עם תחומים מותאמים אישית
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524271"
---
# <a name="set-up-dkim-with-custom-domains"></a>הגדרת DKIM עם תחומים מותאמים אישית

עליך לפרסם שתי רשומות CNAME עבור כל תחום מותאם אישית ב-DNS. לשם כך, השתמש בתבנית הבאה:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **DomainGUID** הוא הטקסט מימין ל **-. mail.protection.outlook.com** ברשומת ה-MX המותאמת אישית עבור התחום המותאם אישית (לדוגמה, contoso-com עבור התחום **contoso.com**). **InitialDomain** הוא התחום שבו השתמשת כאשר נרשמת ל-Office 365 (לדוגמה, **contoso.onmicrosoft.com**).

לקבלת מידע נוסף אודות רשומות DNS, ראה [יצירת רשומות dns בכל ספק אירוח dns עבור Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).