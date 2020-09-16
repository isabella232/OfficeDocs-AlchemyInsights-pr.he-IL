---
title: פרישה של כלי גילוי אלקטרוני מדור קודם
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727784"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="beda0-102">פרישה של כלי גילוי אלקטרוני מדור קודם</span><span class="sxs-lookup"><span data-stu-id="beda0-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="beda0-103">כתוצאה מהפונקציונליות החדשה והמשופרת של גילוי אלקטרוני במרכז התאימות של Microsoft 365, הכלים הבאים של גילוי אלקטרוני ו-commandlet יצאו לגמלאות בחודשים הקרובים:</span><span class="sxs-lookup"><span data-stu-id="beda0-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="beda0-104">[גילוי אלקטרוני](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [ומקום במקום מחזיקים](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) במרכז הניהול של Exchange.</span><span class="sxs-lookup"><span data-stu-id="beda0-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="beda0-105">רכיבי ה-cmdlet של Exchange Online PowerShell התומכים בגילוי אלקטרוני ובמיקום מקומי.</span><span class="sxs-lookup"><span data-stu-id="beda0-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="beda0-106">(רכיבי cmdlet אלה מזוהים באופן קולקטיבי כרכיבי cmdlet \*-MailboxSearch.) הדבר כולל את רכיבי ה-cmdlet הבאים:</span><span class="sxs-lookup"><span data-stu-id="beda0-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="beda0-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="beda0-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="beda0-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="beda0-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="beda0-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="beda0-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="beda0-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="beda0-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="beda0-111">ה [-Cmdlet search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) ב-Microsoft Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="beda0-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="beda0-112">הפעולות הבאות ב-API של Exchange Web Services:</span><span class="sxs-lookup"><span data-stu-id="beda0-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="beda0-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="beda0-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="beda0-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="beda0-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="beda0-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="beda0-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="beda0-116">מתקדם גילוי אלקטרוני v 1.0</span><span class="sxs-lookup"><span data-stu-id="beda0-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="beda0-117">**ציר זמן לפרישה**:</span><span class="sxs-lookup"><span data-stu-id="beda0-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="beda0-118">**התקיימות ב-1 ביולי 2020** לא ניתן עוד ליצור חיפושים וחסימות חדשים, אך באפשרותך לפעול, לערוך ולמחוק חיפושים קיימים באחריותך בלבד.</span><span class="sxs-lookup"><span data-stu-id="beda0-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="beda0-119">התמיכה של Microsoft אינה תומכת עוד במקום ב-גילוי אלקטרוני & המחזיקה ב-EAC.</span><span class="sxs-lookup"><span data-stu-id="beda0-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="beda0-120">ה **-1 באוקטובר 2020** במקום גילוי אלקטרוני & מכיל פונקציונליות ב-EAC ימוקמו במצב קריאה בלבד, כך שתוכל להסיר רק חיפושים וחסימות קיימים.</span><span class="sxs-lookup"><span data-stu-id="beda0-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="beda0-121">**לקבלת מידע נוסף, ראה**:</span><span class="sxs-lookup"><span data-stu-id="beda0-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="beda0-122">העברת חיפושי גילוי אלקטרוני מדור קודם והחסימות למרכז התאימות של Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="beda0-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="beda0-123">פרישה של כלי גילוי אלקטרוני מדור קודם</span><span class="sxs-lookup"><span data-stu-id="beda0-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="beda0-124">שאלות נפוצות אודות גילוי אלקטרוני מקומי ומחזיק מקום במקום</span><span class="sxs-lookup"><span data-stu-id="beda0-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



