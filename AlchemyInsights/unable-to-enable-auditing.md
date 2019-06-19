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
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="e5403-102">אין אפשרות להפעיל ביקורת מאוחד</span><span class="sxs-lookup"><span data-stu-id="e5403-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="e5403-103">כאשר אתה מנסה להפעיל ביקורת אחידה של הארגון Office 365, עשויה להתקבל הודעת שגיאה דומה הבאות:</span><span class="sxs-lookup"><span data-stu-id="e5403-103">When you try to enable unified auditing for your Office 365 organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="e5403-104">כדי לפתור בעיה זו, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="e5403-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="e5403-105">[התחבר להחלפת Powershell מקוון](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="e5403-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="e5403-106">להפעיל cmdlet הבאים:</span><span class="sxs-lookup"><span data-stu-id="e5403-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="e5403-107">המתן עד 60 דקות עבור ההגדרה הקודמת שהשינוי ייכנס לתוקף.</span><span class="sxs-lookup"><span data-stu-id="e5403-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="e5403-108">ב- Exchange Online PowerShell, הפעל את הפקודה הבאה:</span><span class="sxs-lookup"><span data-stu-id="e5403-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="e5403-109">לקבלת מידע נוסף, עיין במאמרים הבאים:</span><span class="sxs-lookup"><span data-stu-id="e5403-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="e5403-110">להתחבר באמצעות אימות מגורמים רבים PowerShell המקוונת של Exchange</span><span class="sxs-lookup"><span data-stu-id="e5403-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="e5403-111">הפעלה או ביטול של חיפוש יומן הביקורת של Office 365</span><span class="sxs-lookup"><span data-stu-id="e5403-111">Turn Office 365 audit log search on or off</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
