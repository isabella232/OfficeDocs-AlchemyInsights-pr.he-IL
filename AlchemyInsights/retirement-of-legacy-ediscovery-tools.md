---
title: פרישה של כלי גילוי אלקטרוני מדור קודם
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798550"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="ddaad-102">פרישה של כלי גילוי אלקטרוני מדור קודם</span><span class="sxs-lookup"><span data-stu-id="ddaad-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="ddaad-103">כתוצאה מהפונקציונליות החדשה והממשופרת של גילוי אלקטרוני במרכז התאימות של Microsoft 365, הכלים והפקודה הבאים של גילוי אלקטרוני מדור קודם יוצאו משימוש בחודשים הקרובים:</span><span class="sxs-lookup"><span data-stu-id="ddaad-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="ddaad-104">[גילוי אלקטרוני במקום והמתנה](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) במקום [במרכז](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) הניהול של Exchange.</span><span class="sxs-lookup"><span data-stu-id="ddaad-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="ddaad-105">כלי ה- cmdlet של PowerShell של Exchange Online התומכים בIn-Place גילוי אלקטרוני In-Place מחזיק.</span><span class="sxs-lookup"><span data-stu-id="ddaad-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="ddaad-106">(כלי cmdlet אלה מזוהים יחד כרכיבי cmdlet של \*-MailboxSearch.) פעולה זו כוללת את כלי ה- cmdlet הבאים:</span><span class="sxs-lookup"><span data-stu-id="ddaad-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="ddaad-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="ddaad-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="ddaad-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="ddaad-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="ddaad-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="ddaad-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="ddaad-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="ddaad-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="ddaad-111">[cmdlet Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) ב- Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ddaad-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="ddaad-112">הפעולות הבאות ב- API של Exchange Web Services:</span><span class="sxs-lookup"><span data-stu-id="ddaad-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="ddaad-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="ddaad-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="ddaad-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="ddaad-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="ddaad-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="ddaad-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="ddaad-116">מתקדם eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="ddaad-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="ddaad-117">**ציר זמן לפרישה**:</span><span class="sxs-lookup"><span data-stu-id="ddaad-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="ddaad-118">**1 ביולי 2020** לא ניתן עוד ליצור חיפושים והחזקות חדשים, אך באפשרותך להפעיל, לערוך ולמחוק חיפושים קיימים על-פי הסיכון שלך.</span><span class="sxs-lookup"><span data-stu-id="ddaad-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="ddaad-119">התמיכה של Microsoft אינה תומכת עוד In-Place גילוי אלקטרוני & ב- EAC.</span><span class="sxs-lookup"><span data-stu-id="ddaad-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="ddaad-120">**1 באוקטובר 2020** In-Place גילוי אלקטרוני & מחזיק פונקציונליות ב- EAC תוצב במצב קריאה בלבד, כך שתוכל להסיר רק חיפושים קיימים והחזקות.</span><span class="sxs-lookup"><span data-stu-id="ddaad-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="ddaad-121">**לקבלת מידע נוסף, ראה**:</span><span class="sxs-lookup"><span data-stu-id="ddaad-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="ddaad-122">העברת חיפושים מדור קודם של גילוי אלקטרוני ונאחזת במרכז התאימות של Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ddaad-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="ddaad-123">פרישה של כלי גילוי אלקטרוני מדור קודם</span><span class="sxs-lookup"><span data-stu-id="ddaad-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="ddaad-124">שאלות נפוצות In-Place גילוי אלקטרוני In-Place מחזיק</span><span class="sxs-lookup"><span data-stu-id="ddaad-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



