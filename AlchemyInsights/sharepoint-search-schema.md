---
title: ניהול סכימת חיפוש ב-SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f2d8d3e07fe32d21af484e4c59e0f5ac6fe8081c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770552"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="ba131-102">ניהול סכימת חיפוש ב-SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="ba131-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="ba131-103">סכימת החיפוש קובעת מה משתמשים יכולים לחפש, כיצד משתמשים יכולים לחפש אותו וכיצד באפשרותך להציג את התוצאות באתרי החיפוש שלך.</span><span class="sxs-lookup"><span data-stu-id="ba131-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="ba131-104">ראה [ניהול סכימת החיפוש ב-SharePoint Online כדי ללמוד כיצד לבצע את הפעולות הבאות](https://docs.microsoft.com/sharepoint/manage-search-schema) :</span><span class="sxs-lookup"><span data-stu-id="ba131-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="ba131-105">שינוי סכימת החיפוש.</span><span class="sxs-lookup"><span data-stu-id="ba131-105">Change the search schema.</span></span>
- <span data-ttu-id="ba131-106">יצירת מאפיינים מנוהלים.</span><span class="sxs-lookup"><span data-stu-id="ba131-106">Create managed properties.</span></span>
- <span data-ttu-id="ba131-107">מיפוי מפה סרוקה מאפיינים סרוקים למאפיינים מנוהלים.</span><span class="sxs-lookup"><span data-stu-id="ba131-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="ba131-108">שים לב לפרטים הבאים לגבי ניהול סכימת החיפוש:</span><span class="sxs-lookup"><span data-stu-id="ba131-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="ba131-109">אם אתה מקבל אזהרה **המציינת שהיישום מושהה** בעת ביצוע שינוי סכימה, הדבר מתבצע רק כאשר קיים תחזוקת שירות שמתרחשת.</span><span class="sxs-lookup"><span data-stu-id="ba131-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="ba131-110">אם חלפו יותר מ-24 שעות ואתה עדיין נתקל באזהרה, התחבר לתיק תמיכה.</span><span class="sxs-lookup"><span data-stu-id="ba131-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="ba131-111">בעת שינוי מאפיינים מנוהלים או הוספת מאפיינים חדשים, השינויים נכנסים לתוקף רק לאחר סריקת התוכן מחדש.</span><span class="sxs-lookup"><span data-stu-id="ba131-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="ba131-112">ב-SharePoint Online, סריקה מתבצעת באופן אוטומטי בהתבסס על לוח הזמנים המוגדר לסריקה.</span><span class="sxs-lookup"><span data-stu-id="ba131-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="ba131-113">כדי לוודא שהשינויים שלך נסרקים, באפשרותך [לבקש במיוחד יצירת אינדקס מחדש של הרשימה או הספריה](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="ba131-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="ba131-114">לקבלת סקירה מלאה של סכימת החיפוש, ראה [הצגת סכימת חיפוש](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="ba131-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


