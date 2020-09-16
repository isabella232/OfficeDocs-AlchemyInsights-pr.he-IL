---
title: 2419-לא ניתן להפוך לזמין-ביקורת
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
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767600"
---
# <a name="unable-to-enable-unified-auditing"></a>לא ניתן להפוך ביקורת מאוחדת לזמינה

כאשר אתה מנסה להפוך ביקורת מאוחדת לזמינה עבור הארגון שלך, אתה עשוי לקבל שגיאה הדומה לשגיאה הבאה:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

כדי לפתור בעיה זו, בצע את הפעולות הבאות:

1. [התחבר אל Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. הפעלת ה-cmdlet הבא:

   ```
   Enable-OrganizationCustomization
   ```

3. המתן עד 60 דקות כדי שההגדרה הקודמת תיכנס לתוקף.

4. הפעלת הפקודה הבאה ב-Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

לקבלת מידע נוסף, עיין במאמרים הבאים:

- [חיבור ל-Exchange Online PowerShell באמצעות אימות רב-גורמי](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [הפעלה או ביטול של חיפוש ביומן הביקורת](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
