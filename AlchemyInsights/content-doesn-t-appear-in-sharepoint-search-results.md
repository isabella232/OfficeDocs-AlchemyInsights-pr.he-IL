---
title: התוכן אינו מופיע בתוצאות החיפוש של SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713131"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="d7202-102">התוכן אינו מופיע בתוצאות החיפוש של SharePoint</span><span class="sxs-lookup"><span data-stu-id="d7202-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="d7202-103">בצע שלבים אלה לפתרון בעיות כאשר תוכן צפוי אינו מופיע בתוצאות החיפוש:</span><span class="sxs-lookup"><span data-stu-id="d7202-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="d7202-104">ודא **שהאתר** המכיל את התוכן הצפוי מוגדר לאפשר לתוכן להופיע בתוצאות חיפוש.</span><span class="sxs-lookup"><span data-stu-id="d7202-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="d7202-105">בצע את השלבים המפורטים [בנושא המציג תוכן באתר בתוצאות חיפוש](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="d7202-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="d7202-106">ודא **שהרשימה** או **הספריה** המכילה את התוכן הצפוי מוגדרים לאפשר לתוכן להופיע בתוצאות חיפוש.</span><span class="sxs-lookup"><span data-stu-id="d7202-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="d7202-107">בצע את השלבים [המפורטים במאמר הצגת תוכן מרשימות או ספריות בתוצאות חיפוש](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="d7202-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="d7202-108">ודא שפריסת הדף, המסמך או העמוד המותאם אישית תפורסם **כגירסה ראשית.**</span><span class="sxs-lookup"><span data-stu-id="d7202-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="d7202-109">בצע את שלב 3 [בחיפוש אינו מחזיר את כל התוצאות ב-SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="d7202-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="d7202-110">ודא שלמשתמש יש **הרשאות** להצגת התוכן.</span><span class="sxs-lookup"><span data-stu-id="d7202-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="d7202-111">בצע את השלבים [בהבנת רמות הרשאה ב-SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="d7202-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="d7202-112">אם סכימת החיפוש השתנתה על-ידי הוספת מאפיין מנוהל חדש, על-ידי עריכת מאפיין מנוהל, או על-ידי הסרת מאפיין מנוהל, לאחר מכן בקשת סריקה ואינדקס מחדש יידרש.</span><span class="sxs-lookup"><span data-stu-id="d7202-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="d7202-113">**צור אינדקס מחדש** של התוכן על-ידי ביצוע השלבים [בבקשה בקשה לסריקה ויצירת אינדקס מחדש של אתר, ספריה או רשימה](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="d7202-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="d7202-114">ייתכן שיידרש זמן מה, המתן 24 שעות לפני שתבדוק שוב את התוצאות.</span><span class="sxs-lookup"><span data-stu-id="d7202-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="d7202-115">לקבלת מידע נוסף, ראה [הפיכת תוכן לזמין באתר לניתן לחיפוש](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="d7202-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
