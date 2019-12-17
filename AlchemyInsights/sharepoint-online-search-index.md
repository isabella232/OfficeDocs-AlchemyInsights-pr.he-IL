---
title: חפש ב-SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044044"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="2569f-102">תוכן סריקה ויצירת אינדקס ב-SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="2569f-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="2569f-103">יש לסרוק את התוכן ולהוסיף אותו לאינדקס החיפוש כדי שהמשתמשים ימצאו את מה שהם מחפשים ב-SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="2569f-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="2569f-104">התוכן נסרק באופן אוטומטי על בסיס לוח זמנים לסריקה שהוגדר מראש (אין אפשרות לשנות את לוח הזמנים לסריקה).</span><span class="sxs-lookup"><span data-stu-id="2569f-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="2569f-105">הסורק מרים תוכן שהשתנה מאז הסריקה האחרונה ומעדכן את האינדקס.</span><span class="sxs-lookup"><span data-stu-id="2569f-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="2569f-106">כדי להבטיח שהתוכן ייסרק והאינדקס יעודכן, שים לב לפרטים הבאים:</span><span class="sxs-lookup"><span data-stu-id="2569f-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="2569f-107">ודא שניתן למצוא תוכן על-ידי [הפיכת תוכן האתר לחיפוש](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="2569f-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="2569f-108">לאחר ששינית מאפיין מנוהל, או כאשר שינית את המיפוי של מאפיינים סרוקים ומנוהלים, יש לסרוק מחדש את האתר לפני שהשינויים ישתקפו באינדקס החיפוש.</span><span class="sxs-lookup"><span data-stu-id="2569f-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="2569f-109">מכיוון שהשינויים שלך נעשים בסכימת החיפוש, ולא באתר בפועל, הסורק לא יחדש באופן אוטומטי את האתר באינדקס.</span><span class="sxs-lookup"><span data-stu-id="2569f-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="2569f-110">לקבלת מידע נוסף, ראה [בקשה ידנית לסריקה וליצירת אינדקס מחדש של אתר, ספריה או רשימה](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="2569f-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="2569f-111">המתן 24 שעות לפחות לאחר בקשה ידנית לסריקה ולאינדקס מחדש מלא כדי לראות אם אתה עדיין נתקל בבעיה.</span><span class="sxs-lookup"><span data-stu-id="2569f-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="2569f-112">אם חלפו יותר מ -24 שעות מאז התחלת הסריקה והאינדקס החדש המלא, נא לרשום מקרה תמיכה.</span><span class="sxs-lookup"><span data-stu-id="2569f-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="2569f-113">במקרים רבים, אנחנו כבר עובדים על פתרון.</span><span class="sxs-lookup"><span data-stu-id="2569f-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="2569f-114">בבקשה תן לנו לפחות 24. שעות כדי להשלים פיתרון</span><span class="sxs-lookup"><span data-stu-id="2569f-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="2569f-115">אם אתר, מסמך (ספריה) או רשימה נמחקו ועדיין מוצגים בתוצאות החיפוש, על המשתמשים לקבל **שגיאה 404 קובץ לא נמצא** בעת ניסיון לגשת אליו.</span><span class="sxs-lookup"><span data-stu-id="2569f-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="2569f-116">בעיה זו צריכה להירשם כמקרה תמיכה עבור חקירה נוספת.</span><span class="sxs-lookup"><span data-stu-id="2569f-116">This issue should be logged as a support case for further investigation.</span></span> 



