---
title: ניהול סכימת חיפוש ב-SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 9836cf139e97fc556995a8f0ad38c51c5c2392ac
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042964"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="980f3-102">ניהול סכימת חיפוש ב-SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="980f3-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="980f3-103">סכימת החיפוש קובעת אילו משתמשים יכולים לחפש, כיצד משתמשים יכולים לחפש אותו וכיצד ניתן להציג את התוצאות באתרי האינטרנט של החיפוש.</span><span class="sxs-lookup"><span data-stu-id="980f3-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="980f3-104">ראה [ניהול סכימת החיפוש ב-SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) כדי ללמוד כיצד:</span><span class="sxs-lookup"><span data-stu-id="980f3-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="980f3-105">שנה את סכימת החיפוש.</span><span class="sxs-lookup"><span data-stu-id="980f3-105">Change the search schema.</span></span>
- <span data-ttu-id="980f3-106">צור מאפיינים מנוהלים.</span><span class="sxs-lookup"><span data-stu-id="980f3-106">Create managed properties.</span></span>
- <span data-ttu-id="980f3-107">מפה של המפה הסרוקים מאפיינים סרוקים למאפיינים מנוהלים.</span><span class="sxs-lookup"><span data-stu-id="980f3-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="980f3-108">שים לב לפרטים הבאים בנוגע לניהול סכימת החיפוש שלך:</span><span class="sxs-lookup"><span data-stu-id="980f3-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="980f3-109">אם מתקבלת אזהרה **המציינת שהיישום מושהה** בעת ביצוע שינוי סכימה, הדבר מתרחש רק באופן זמני כאשר התרחשות תחזוקת שירות.</span><span class="sxs-lookup"><span data-stu-id="980f3-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="980f3-110">אם חלפו יותר מ -24 שעות ועדיין חווית את האזהרה, נא לרשום מקרה תמיכה.</span><span class="sxs-lookup"><span data-stu-id="980f3-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="980f3-111">בעת שינוי מאפיינים מנוהלים או הוספת כאלה חדשים, השינויים ייכנסו לתוקף רק לאחר שהתוכן נסרק מחדש.</span><span class="sxs-lookup"><span data-stu-id="980f3-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="980f3-112">ב-SharePoint Online, הסריקה מתרחשת באופן אוטומטי בהתבסס על לוח הזמנים המוגדר לסריקה.</span><span class="sxs-lookup"><span data-stu-id="980f3-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="980f3-113">כדי לוודא שהשינויים שלך נסרקים, באפשרותך [לבקש במפורש יצירת אינדקס מחדש של הרשימה או הספריה](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="980f3-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="980f3-114">לקבלת סקירה מלאה של סכימת החיפוש, ראה [הצגת סכימת החיפוש](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="980f3-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


