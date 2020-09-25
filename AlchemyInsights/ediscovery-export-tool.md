---
title: כלי הייצוא של גילוי אלקטרוני
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277933"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="b6745-102">לא ניתן להתקין או להפעיל את כלי הייצוא של גילוי אלקטרוני?</span><span class="sxs-lookup"><span data-stu-id="b6745-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="b6745-103">אם אינך מצליח להתקין או להפעיל את כלי הייצוא של גילוי אלקטרוני כדי להוריד תוצאות חיפוש, בדוק את הדברים הבאים:</span><span class="sxs-lookup"><span data-stu-id="b6745-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="b6745-104">המחשב שבו אתה משתמש עומד בדרישות הדרישות המוקדמות הבאות:</span><span class="sxs-lookup"><span data-stu-id="b6745-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="b6745-105">גירסאות 32 או 64 סיביות של Windows 7 וגירסאות מתקדמות יותר</span><span class="sxs-lookup"><span data-stu-id="b6745-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="b6745-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="b6745-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="b6745-107">דפדפן נתמך:</span><span class="sxs-lookup"><span data-stu-id="b6745-107">A supported browser:</span></span>

  - <span data-ttu-id="b6745-108">מייקרוסופט אדג'</span><span class="sxs-lookup"><span data-stu-id="b6745-108">Microsoft Edge</span></span>

    <span data-ttu-id="b6745-109">או</span><span class="sxs-lookup"><span data-stu-id="b6745-109">Or</span></span>

  - <span data-ttu-id="b6745-110">Internet Explorer 10 וגירסאות מתקדמות יותר</span><span class="sxs-lookup"><span data-stu-id="b6745-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="b6745-111">דפדפנים אחרים, כגון Google Chrome ו-Mozilla Firefox אינם נתמכים.</span><span class="sxs-lookup"><span data-stu-id="b6745-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="b6745-112">הארגון שלך יכול להתחבר לנקודת הקצה בתכלת, שהיא \*\* \* . blob.core.windows.net\*\* (התווים הכלליים מייצגים מזהה ייחודי עבור משימת הייצוא שלך).</span><span class="sxs-lookup"><span data-stu-id="b6745-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="b6745-113">מוקצית לך תפקיד הייצוא במרכז תאימות האבטחה של Microsoft 365 &amp; .</span><span class="sxs-lookup"><span data-stu-id="b6745-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="b6745-114">כברירת מחדל, תפקיד זה מוקצה רק לקבוצת התפקידים של גילוי אלקטרוני Manager.</span><span class="sxs-lookup"><span data-stu-id="b6745-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="b6745-115">ראה [הקצאת הרשאות גילוי אלקטרוני](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="b6745-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="b6745-116">לקבלת מידע נוסף, ראה [ייצוא תוצאות חיפוש תוכן](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="b6745-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="b6745-117">אם אתה מייצא יותר מ-100 תיבות דואר, יהיה עליך להשתמש ב-Powershell הבאים כדי להוריד את תוצאות הייצוא:  [ייצוא תוצאות של יותר מ-100 תיבות דואר](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="b6745-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>