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
ms.openlocfilehash: cb1f621dffc88464c339b55998efb5440cfd775c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332308"
---
# <a name="set-up-dkim-with-custom-domains"></a>הגדרת DKIM עם תחומים מותאמים אישית

עליך לפרסם שתי רשומות CNAME עבור כל תחום מותאם אישית ב- DNS. לשם כך, השתמש בתבנית הבאה:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
**הערה:** **DomainGUID** הוא הטקסט מימין **ל- .mail.protection.outlook.com ברשומת** MX המותאמת אישית עבור התחום המותאם אישית (לדוגמה, contoso-com **עבור התחום contoso.com).** **InitialDomain** הוא התחום שהשתמשת בו כאשר נרשמת Office 365 (לדוגמה, **contoso.onmicrosoft.com**).

לקבלת מידע נוסף אודות רשומות DNS, ראה [יצירת רשומות DNS בכל ספק אירוח DNS עבור Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).