---
title: תוכן אינו מופיע בתוצאות החיפוש של SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: 8215b0a5cde5adffa3bec37d6699418557f914dd
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35363808"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="0bc94-102">תוכן אינו מופיע בתוצאות החיפוש של SharePoint</span><span class="sxs-lookup"><span data-stu-id="0bc94-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="0bc94-103">בצע את שלבי פתרון הבעיות כאשר תוכן הצפוי אינו מופיע בתוצאות החיפוש:</span><span class="sxs-lookup"><span data-stu-id="0bc94-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="0bc94-104">בדוק **האתר** המכיל את התוכן הצפוי מוגדר לאפשר תוכן יופיעו בתוצאות החיפוש.</span><span class="sxs-lookup"><span data-stu-id="0bc94-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="0bc94-105">בצע את השלבים ב [הצג תוכן באתר בתוצאות החיפוש](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="0bc94-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="0bc94-106">בדוק **הרשימה** או את **הספריה** המכילה את התוכן הצפוי מוגדר לאפשר תוכן יופיעו בתוצאות החיפוש.</span><span class="sxs-lookup"><span data-stu-id="0bc94-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="0bc94-107">בצע את השלבים ב [הצג תוכן מרשימות או מספריות בתוצאות החיפוש](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="0bc94-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="0bc94-108">ודא הדף, על המסמך או על פריסת עמוד מותאם אישית שתפורסם כ **גירסה ראשית.**</span><span class="sxs-lookup"><span data-stu-id="0bc94-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="0bc94-109">בצע את שלב 3 בחלונית [החיפוש אינה מחזירה את כל התוצאות ב- SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="0bc94-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="0bc94-110">ודא שלמשתמש יש **הרשאות** להציג את התוכן.</span><span class="sxs-lookup"><span data-stu-id="0bc94-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="0bc94-111">בצע את השלבים בנושא [הכרת רמות הרשאה ב- SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="0bc94-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="0bc94-112">אם סכימת החיפוש שונתה על-ידי הוספת מאפיין מנוהל חדש, על-ידי עריכת מאפיין מנוהל או על-ידי הסרת מאפיין מנוהל מכן מבקש סריקה אינדקס מחדש יהיה צורך.</span><span class="sxs-lookup"><span data-stu-id="0bc94-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="0bc94-113">**אינדקס מחדש** התוכן על-ידי ביצוע השלבים בנושא [לבקש באופן ידני סריקה ויצירת אינדקס מחדש של אתר, ספריה או רשימה](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="0bc94-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="0bc94-114">הדבר עלול להימשך זמן רב, המתן 24 שעות לפני בדיקת התוצאות שוב.</span><span class="sxs-lookup"><span data-stu-id="0bc94-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="0bc94-115">לקבלת מידע נוסף, ראה [הפעלת תוכן באתר כדי לשמש בחיפושים](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="0bc94-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
