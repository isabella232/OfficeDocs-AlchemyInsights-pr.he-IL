---
title: 2419-אין אפשרות-אל-אפשר-ביקורת
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065649"
---
# <a name="unable-to-enable-unified-auditing"></a>אין אפשרות להפעיל ביקורת מאוחד

כאשר אתה מנסה להפעיל ביקורת אחידה של הארגון Office 365, עשויה להתקבל הודעת שגיאה דומה הבאות:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

כדי לפתור בעיה זו, בצע את הפעולות הבאות:

1. [התחבר להחלפת Powershell מקוון](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. להפעיל cmdlet הבאים:

   ```
   Enable-OrganizationCustomization
   ```

3. המתן עד 60 דקות עבור ההגדרה הקודמת שהשינוי ייכנס לתוקף.

4. ב- Exchange Online PowerShell, הפעל את הפקודה הבאה:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

לקבלת מידע נוסף, עיין במאמרים הבאים:

- [להתחבר באמצעות אימות מגורמים רבים PowerShell המקוונת של Exchange](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [הפעלה או ביטול של חיפוש יומן הביקורת של Office 365](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
