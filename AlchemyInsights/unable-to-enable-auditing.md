---
title: 2419-unable-to-enable-auditing
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 0566a8d002b1bd9e38f3184824193394e49d56494d347338f96cfcdfdb758f4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007791"
---
# <a name="unable-to-enable-unified-auditing"></a>לא ניתן להפוך ביקורת מאוחדת לזמינה

בעת ניסיון להפוך ביקורת מאוחדת לזמינה עבור הארגון שלך, ייתכן שתקבל שגיאה הדומה לשגיאה הבאה:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

כדי לפתור בעיה זו, בצע את הפעולות הבאות:

1. [התחברות כדי Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. הפעל את ה- cmdlet הבא:

   ```
   Enable-OrganizationCustomization
   ```

3. המתן 60 דקות עד שההגדרה הקודמת תוקף.

4. הפעל את הפקודה הבאה ב- Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

לקבלת מידע נוסף, עיין במאמרים הבאים:

- [התחברות כדי Exchange Online PowerShell באמצעות אימות רב-גורמי](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [הפעלה או ביטול של חיפוש ביומן ביקורת](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
