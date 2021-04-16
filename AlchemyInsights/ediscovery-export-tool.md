---
title: כלי ייצוא גילוי אלקטרוני
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814589"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="cfc00-102">לא ניתן להתקין או להפעיל את כלי הייצוא של גילוי אלקטרוני?</span><span class="sxs-lookup"><span data-stu-id="cfc00-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="cfc00-103">אם אינך יכול להתקין או להפעיל את כלי הייצוא של גילוי אלקטרוני כדי להוריד תוצאות חיפוש, בדוק את הדברים הבאים:</span><span class="sxs-lookup"><span data-stu-id="cfc00-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="cfc00-104">המחשב שבו אתה משתמש ייפגש עם דרישות מוקדמות אלה:</span><span class="sxs-lookup"><span data-stu-id="cfc00-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="cfc00-105">גירסאות 32 או 64 סיביות של Windows 7 וגירסאות מתקדמות יותר</span><span class="sxs-lookup"><span data-stu-id="cfc00-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="cfc00-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="cfc00-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="cfc00-107">דפדפן נתמך:</span><span class="sxs-lookup"><span data-stu-id="cfc00-107">A supported browser:</span></span>

  - <span data-ttu-id="cfc00-108">מייקרוסופט אדג'</span><span class="sxs-lookup"><span data-stu-id="cfc00-108">Microsoft Edge</span></span>

    <span data-ttu-id="cfc00-109">או</span><span class="sxs-lookup"><span data-stu-id="cfc00-109">Or</span></span>

  - <span data-ttu-id="cfc00-110">Internet Explorer 10 וגירסאות מתקדמות יותר</span><span class="sxs-lookup"><span data-stu-id="cfc00-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="cfc00-111">דפדפנים אחרים, כגון Google Chrome ו- Mozilla Firefox אינם נתמכים.</span><span class="sxs-lookup"><span data-stu-id="cfc00-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="cfc00-112">הארגון שלך יכול להתחבר אל נקודת הקצה ב- Azure, **\* שהיא .blob.core.windows.net** (תו כללי מייצג מזהה ייחודי עבור עבודת הייצוא שלך).</span><span class="sxs-lookup"><span data-stu-id="cfc00-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="cfc00-113">מוקצה לך תפקיד ייצוא במרכז תאימות האבטחה של Microsoft 365. &amp;</span><span class="sxs-lookup"><span data-stu-id="cfc00-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="cfc00-114">כברירת מחדל, תפקיד זה מוקצה רק לקבוצת התפקידים של מנהל גילוי אלקטרוני.</span><span class="sxs-lookup"><span data-stu-id="cfc00-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="cfc00-115">ראה [הקצאת הרשאות גילוי אלקטרוני](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="cfc00-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="cfc00-116">לקבלת מידע נוסף, ראה [ייצוא תוצאות חיפוש תוכן](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="cfc00-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="cfc00-117">אם אתה מייצא יותר מ- 100,000 תיבות דואר, יהיה עליך להשתמש ב- Powershell הבא כדי להוריד את תוצאות הייצוא: ייצוא תוצאות ביותר מתיבות דואר של  [100K](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="cfc00-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>