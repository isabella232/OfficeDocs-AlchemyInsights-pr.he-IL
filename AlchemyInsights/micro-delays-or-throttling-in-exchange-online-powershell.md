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
ms.openlocfilehash: 680df9e6e2404ff6b60b17d6ac88e202e9a7bb25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830034"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="a5092-102">מיקרו עיכובים או ויסות ב- Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="a5092-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="a5092-103">ייתכן שתראה אזהרות "מיקרו עיכוב הוחל" או עיכובים כאשר בעת הפעלת קובצי Script או cmdlets ב- Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="a5092-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="a5092-104">להלן שתי הצעות הקשורות לכך:</span><span class="sxs-lookup"><span data-stu-id="a5092-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="a5092-105">ייתכן שתרצה לנסות להשתמש ב[מודול Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), הכולל את רכיבי ה-CMDlet המבוססים על REST API ובעלי ביצועים טובים יותר באופן משמעותי.</span><span class="sxs-lookup"><span data-stu-id="a5092-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="a5092-106">פעולה זו עשויה להיות פתרון מצוין עבור רכיבי Get- CMDlets רבים שנמצאים בשימוש לעיתים קרובות.</span><span class="sxs-lookup"><span data-stu-id="a5092-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="a5092-107">אם עליך להשתמש ברכיבי CMDlet שאינם מכוסים עדיין במודול v2, ראה את הנושא [הפעלה באמצעות רכיבי cmdlet של PowerShell עבור מספר גדול של משתמשים ב- Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), שדן בכיצד ניתן לעקוף מגבלות ויסות צפויות של PowerShell ב- Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="a5092-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>
