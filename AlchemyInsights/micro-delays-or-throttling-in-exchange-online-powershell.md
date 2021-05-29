---
title: מיקרו עיכובים או ויסות ב- Exchange Online PowerShell
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
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702127"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="caf62-102">מיקרו עיכובים או ויסות ב- Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="caf62-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="caf62-103">ייתכן שתראה אזהרות "מיקרו עיכוב הוחל" או עיכובים כאשר בעת הפעלת קובצי Script או cmdlets ב- Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="caf62-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="caf62-104">להלן כמה הצעות כיצד לפתור את הבעיה:</span><span class="sxs-lookup"><span data-stu-id="caf62-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="caf62-105">הפעל את האבחון שלנו כדי להירגע מדיניות ויסות PowerShell של הדייר שלך.</span><span class="sxs-lookup"><span data-stu-id="caf62-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="caf62-106">פתרון זה יפתור את הבעיה לרוב.</span><span class="sxs-lookup"><span data-stu-id="caf62-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="caf62-107">אם הבעיה עדיין לא נפתרה, [השתמש במודול Exchange Online v2 PowerShell](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), הכולל כלי CMDlet המבוססים על REST API והם מבצעים באופן משמעותי יותר.</span><span class="sxs-lookup"><span data-stu-id="caf62-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="caf62-108">פעולה זו עשויה להיות פתרון מצוין עבור רכיבי Get- CMDlets רבים שנמצאים בשימוש לעיתים קרובות.</span><span class="sxs-lookup"><span data-stu-id="caf62-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="caf62-109">אם עליך להשתמש ברכיבי CMDlet שלא מכוסים במודול v2, ראה הפעלת [כלי cmdlet](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)של PowerShell עבור מספר גדול של משתמשים ב- Office 365 , אשר מדבר על האופן שבו ניתן לעקוף את מגבלות ויסות PowerShell ב- Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="caf62-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
