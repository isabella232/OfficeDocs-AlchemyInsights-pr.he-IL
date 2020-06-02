---
title: 2419-אין אפשרות לאפשר-ביקורת
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510429"
---
# <a name="unable-to-enable-unified-auditing"></a>אין אפשרות להפוך ביקורת אחידה לזמינה

כאשר אתה מנסה להפוך ביקורת אחידה לזמינה עבור הארגון שלך, ייתכן שתתקבל שגיאה בדומה לשגיאה הבאה:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

כדי לפתור בעיה זו, בצע את הפעולות הבאות:

1. [להתחבר ל-Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. הפעל את ה-cmdlet הבא:

   ```
   Enable-OrganizationCustomization
   ```

3. המתן 60 דקות כדי שההגדרה הקודמת ייכנסו לתוקף.

4. הפעל את הפקודה הבאה ב-Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

לקבלת מידע נוסף, עיין במאמרים הבאים:

- [התחבר ל-Exchange Online PowerShell באמצעות אימות מרובה גורמים](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [הפעלה או ביטול של חיפוש ביומן הביקורת](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
