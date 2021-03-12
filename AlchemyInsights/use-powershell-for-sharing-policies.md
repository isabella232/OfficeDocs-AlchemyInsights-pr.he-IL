---
title: שימוש ב- PowerShell לשיתוף פריטי מדיניות וקשרים ארגוניים
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: cd1d34e4dae474e61c799ca9234b2f18c718f27b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709467"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>שימוש ב- PowerShell לשיתוף פריטי מדיניות וקשרים ארגוניים


עבור קשרים ארגוניים, עיין בתחביר המפורט ובפרטי הפרמטר עבור : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  ו-  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

כדי ליצור מדיניות שיתוף, השתמש ב[New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). כדי  [להחיל מדיניות שיתוף על תיבת דואר או על משתמש](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  עליך להשתמש בשילוב של  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) ו- [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) עם המדיניות החדשה שנוצרה. כדי  [לשנות, לבטל או להסיר מדיניות שיתוף](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  עליך להשתמש ב-  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) וב- [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**כדי להבין את הנושא הזה במלואו, קרא את הבאים:**

[שיתוף ב- Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)