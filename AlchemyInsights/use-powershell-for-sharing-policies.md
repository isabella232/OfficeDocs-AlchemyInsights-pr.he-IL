---
title: השתמש ב-PowerShell לשיתוף מדיניות וקשרי גומלין בין ארגונים
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862087"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="89c92-102">השתמש ב-PowerShell לשיתוף מדיניות וקשרי גומלין בין ארגונים</span><span class="sxs-lookup"><span data-stu-id="89c92-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="89c92-103">עבור קשרי גומלין בין ארגונים, עיין בתחביר ובמידע הפרמטרים המפורטים עבור: [מידע מקבל-הפדרלי](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [קשרי גומלין של ארגון חדש](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [קשרי גומלין מוגדרים](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) [והסרת קשר](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship)ארגוני.</span><span class="sxs-lookup"><span data-stu-id="89c92-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="89c92-104">כדי ליצור שימוש במדיניות שיתוף השתמש [במדיניות חדשה](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy)לשיתוף.</span><span class="sxs-lookup"><span data-stu-id="89c92-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="89c92-105">כדי [להחיל מדיניות שיתוף על תיבת דואר או על משתמש](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) שעליך להשתמש בשילוב של [תיבת דואר](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) [ולקבל תיבת דואר](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) עם המדיניות החדשה שנוצרה.</span><span class="sxs-lookup"><span data-stu-id="89c92-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="89c92-106">כדי [לשנות, להשבית או להסיר מדיניות שיתוף](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) עליך להשתמש [במדיניות Set-sharingpolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) [ולהסיר את המדיניות](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="89c92-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="89c92-107">**לקבלת הבנה מלאה של נושא זה נא לקרוא:**</span><span class="sxs-lookup"><span data-stu-id="89c92-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="89c92-108">שיתוף ב-Exchange Online</span><span class="sxs-lookup"><span data-stu-id="89c92-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)