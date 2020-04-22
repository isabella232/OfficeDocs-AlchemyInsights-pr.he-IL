---
title: התוכן אינו מופיע בתוצאות החיפוש של SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a21e0047b41390f740f9e13d31cba32b13990151
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705662"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="4a847-102">התוכן אינו מופיע בתוצאות החיפוש של SharePoint</span><span class="sxs-lookup"><span data-stu-id="4a847-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="4a847-103">בצע את הפעולות לפתרון בעיות אלה כאשר תוכן צפוי אינו מופיע בתוצאות החיפוש:</span><span class="sxs-lookup"><span data-stu-id="4a847-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="4a847-104">ודא **שהאתר** המכיל את התוכן הצפוי מוגדר כך שיאפשר לתוכן להופיע בתוצאות חיפוש.</span><span class="sxs-lookup"><span data-stu-id="4a847-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="4a847-105">בצע את השלבים [בהצגת תוכן באתר בתוצאות חיפוש](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="4a847-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="4a847-106">בדוק **שהרשימה** או **הספריה** המכילה את התוכן הצפוי מוגדרות כדי לאפשר לתוכן להופיע בתוצאות חיפוש.</span><span class="sxs-lookup"><span data-stu-id="4a847-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="4a847-107">בצע את השלבים [בהצגת תוכן מרשימות או ספריות בתוצאות חיפוש](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="4a847-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="4a847-108">ודא שפריסת הדף, המסמך או העמוד המותאם אישית מתפרסמת **כגירסה ראשית.**</span><span class="sxs-lookup"><span data-stu-id="4a847-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="4a847-109">בצע את שלב 3 [בחיפוש אינו מחזיר את כל התוצאות ב-SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="4a847-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="4a847-110">ודא שלמשתמש יש **הרשאות** להציג את התוכן.</span><span class="sxs-lookup"><span data-stu-id="4a847-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="4a847-111">בצע את השלבים [בהבנת רמות ההרשאה ב-SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="4a847-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="4a847-112">אם סכימת החיפוש שונתה על-ידי הוספת מאפיין מנוהל חדש, על-ידי עריכת מאפיין מנוהל, או על-ידי הסרת מאפיין מנוהל ולאחר מכן תתבקש לבצע סריקה ואינדקס מחדש.</span><span class="sxs-lookup"><span data-stu-id="4a847-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="4a847-113">**צור אינדקס מחדש** של התוכן על-ידי ביצוע השלבים [בבקשה ידנית של סריקה ויצירת אינדקס מחדש של אתר, ספריה או רשימה](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="4a847-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="4a847-114">הדבר עלול להימשך זמן מה, להמתין 24 שעות לפני בדיקת התוצאות שוב.</span><span class="sxs-lookup"><span data-stu-id="4a847-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="4a847-115">לקבלת מידע נוסף, ראה [הפיכת תוכן באתר לזמין לחיפוש](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="4a847-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
