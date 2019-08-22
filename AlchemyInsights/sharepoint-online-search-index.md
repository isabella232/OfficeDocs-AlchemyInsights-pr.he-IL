---
title: חיפוש ב- SharePoint באופן מקוון
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 3c3f6384172b2b4d59db6059618572db11059228
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507632"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="b0cb4-102">סריקת תוכן ואינדקס ב- SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="b0cb4-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="b0cb4-103">חייב להיות סרוקים ותוכן נוסף לאינדקס החיפוש עבור משתמשים למצוא את מה שהם שאתה מחפש ב- SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="b0cb4-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="b0cb4-104">התוכן נסרק באופן אוטומטי בהתבסס על לוח זמנים לסריקה מוגדרים מראש (אין אפשרות לשנות את לוח הזמנים של סריקה).</span><span class="sxs-lookup"><span data-stu-id="b0cb4-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="b0cb4-105">הסורק ידגום תוכן השתנה מאז הסריקה האחרונה ומעדכנת את האינדקס.</span><span class="sxs-lookup"><span data-stu-id="b0cb4-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="b0cb4-106">כדי להבטיח התוכן נסרק שהאינדקס יתעדכן, שים לב לדברים הבאים:</span><span class="sxs-lookup"><span data-stu-id="b0cb4-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="b0cb4-107">ודא כי ניתן למצוא תוכן על-ידי [הפיכת אתר תוכן הניתן לחיפוש](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="b0cb4-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="b0cb4-108">שינית מאפיין מנוהל, או שינית את המיפוי של סרוקים והניהול של מאפיינים, האתר חייב להיות סרוק מחדש לפני שהשינויים ישתקפו באינדקס החיפוש.</span><span class="sxs-lookup"><span data-stu-id="b0cb4-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="b0cb4-109">מכיוון שהשינויים שלך נעשים סכימת החיפוש, לא לאתר בפועל, תביא הסורק באופן אוטומטי אינדקס מחדש את האתר.</span><span class="sxs-lookup"><span data-stu-id="b0cb4-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="b0cb4-110">לקבלת מידע נוסף, ראה [לבקש באופן ידני סריקה ויצירת אינדקס מחדש של אתר, ספריה או רשימה](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="b0cb4-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="b0cb4-111">המתן לפחות 24 שעות לאחר מבקש באופן ידני של הסריקה ואינדקס מלא מחדש כדי לראות אם אתה עדיין נתקל בבעיה.</span><span class="sxs-lookup"><span data-stu-id="b0cb4-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="b0cb4-112">אם יותר מ- 24 שעות חלפו מאז יזם את הסריקה ואינדקס מלא מחדש, היכנס אירוע תמיכה.</span><span class="sxs-lookup"><span data-stu-id="b0cb4-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="b0cb4-113">במקרים רבים, אנו אתה כבר עובד על פתרון.</span><span class="sxs-lookup"><span data-stu-id="b0cb4-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="b0cb4-114">נא תן לנו לפחות 24 שעות להשלמת פתרון.</span><span class="sxs-lookup"><span data-stu-id="b0cb4-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="b0cb4-115">אם אתר, מסמך (ספריה), או רשימה נמחק ומציג עדיין בתוצאות החיפוש, משתמשים אמורה להתקבל **שגיאה 404 קובץ לא נמצא** בעת ניסיון לגשת אליו.</span><span class="sxs-lookup"><span data-stu-id="b0cb4-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="b0cb4-116">בעיה זו עליך להיכנס אירוע תמיכה לצורך בדיקה נוספת.</span><span class="sxs-lookup"><span data-stu-id="b0cb4-116">This issue should be logged as a support case for further investigation.</span></span> 



