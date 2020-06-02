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
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="1e0d1-102">אין אפשרות להפוך ביקורת אחידה לזמינה</span><span class="sxs-lookup"><span data-stu-id="1e0d1-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="1e0d1-103">כאשר אתה מנסה להפוך ביקורת אחידה לזמינה עבור הארגון שלך, ייתכן שתתקבל שגיאה בדומה לשגיאה הבאה:</span><span class="sxs-lookup"><span data-stu-id="1e0d1-103">When you try to enable unified auditing for your organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="1e0d1-104">כדי לפתור בעיה זו, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="1e0d1-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="1e0d1-105">[להתחבר ל-Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="1e0d1-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="1e0d1-106">הפעל את ה-cmdlet הבא:</span><span class="sxs-lookup"><span data-stu-id="1e0d1-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="1e0d1-107">המתן 60 דקות כדי שההגדרה הקודמת ייכנסו לתוקף.</span><span class="sxs-lookup"><span data-stu-id="1e0d1-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="1e0d1-108">הפעל את הפקודה הבאה ב-Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="1e0d1-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="1e0d1-109">לקבלת מידע נוסף, עיין במאמרים הבאים:</span><span class="sxs-lookup"><span data-stu-id="1e0d1-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="1e0d1-110">התחבר ל-Exchange Online PowerShell באמצעות אימות מרובה גורמים</span><span class="sxs-lookup"><span data-stu-id="1e0d1-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="1e0d1-111">הפעלה או ביטול של חיפוש ביומן הביקורת</span><span class="sxs-lookup"><span data-stu-id="1e0d1-111">Turn audit log search on or off</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
