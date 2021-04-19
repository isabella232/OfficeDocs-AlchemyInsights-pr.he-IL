---
title: שימוש ב- PowerShell לשיתוף פריטי מדיניות וקשרים ארגוניים
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 9c52b876160f9577e6cefe7644c29d6fdf3b23fd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826056"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="6d8fd-102">שימוש ב- PowerShell לשיתוף פריטי מדיניות וקשרים ארגוניים</span><span class="sxs-lookup"><span data-stu-id="6d8fd-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="6d8fd-103">עבור קשרים ארגוניים, עיין בתחביר המפורט ובפרטי הפרמטר עבור : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  ו-  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="6d8fd-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="6d8fd-104">כדי ליצור מדיניות שיתוף, השתמש ב[New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="6d8fd-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="6d8fd-105">כדי  [להחיל מדיניות שיתוף על תיבת דואר או על משתמש](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  עליך להשתמש בשילוב של  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) ו- [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) עם המדיניות החדשה שנוצרה.</span><span class="sxs-lookup"><span data-stu-id="6d8fd-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="6d8fd-106">כדי  [לשנות, לבטל או להסיר מדיניות שיתוף](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  עליך להשתמש ב-  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) וב- [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="6d8fd-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="6d8fd-107">**כדי להבין את הנושא הזה במלואו, קרא את הבאים:**</span><span class="sxs-lookup"><span data-stu-id="6d8fd-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="6d8fd-108">שיתוף ב- Exchange Online</span><span class="sxs-lookup"><span data-stu-id="6d8fd-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)