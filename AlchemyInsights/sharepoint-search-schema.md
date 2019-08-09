---
title: ניהול סכימת החיפוש ב- SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f49195bec64f115063ccfb5256e27fbecd4a54f6
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270106"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="29cf4-102">ניהול סכימת החיפוש ב- SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="29cf4-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="29cf4-103">סכימת החיפוש מבקרת מה המשתמשים יכולים לחפש, כיצד משתמשים יכולים לחפש אותו, כיצד ניתן להציג את התוצאות באתרי החיפוש שלך.</span><span class="sxs-lookup"><span data-stu-id="29cf4-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="29cf4-104">ראה [ניהול סכימת החיפוש ב- SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) כדי ללמוד כיצד:</span><span class="sxs-lookup"><span data-stu-id="29cf4-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="29cf4-105">לשנות את סכימת החיפוש.</span><span class="sxs-lookup"><span data-stu-id="29cf4-105">Change the search schema.</span></span>
- <span data-ttu-id="29cf4-106">יצירת מאפיינים מנוהלים.</span><span class="sxs-lookup"><span data-stu-id="29cf4-106">Create managed properties.</span></span>
- <span data-ttu-id="29cf4-107">מפת סרוקים מפת מאפיינים סרוקים אל מאפיינים מנוהלים.</span><span class="sxs-lookup"><span data-stu-id="29cf4-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="29cf4-108">שים לב לנקודות הבאות בקובץ מתייחסת לניהול סכימת החיפוש שלך:</span><span class="sxs-lookup"><span data-stu-id="29cf4-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="29cf4-109">אם תקבל אזהרה המציינת **שהיישום מושהה** בעת ביצוע שינוי הסכימה, זהו רק זמני שכן אין שירות תחזוקה המתרחשים.</span><span class="sxs-lookup"><span data-stu-id="29cf4-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="29cf4-110">אם חלפו יותר מ- 24 שעות ולחוות מחדש את האזהרה עדיין, היכנס אירוע תמיכה.</span><span class="sxs-lookup"><span data-stu-id="29cf4-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="29cf4-111">בעת שינוי מאפיינים מנוהלים או להוסיף חדשים, השינויים ייכנסו לתוקף רק לאחר התוכן שנסרק מחדש.</span><span class="sxs-lookup"><span data-stu-id="29cf4-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="29cf4-112">ב- SharePoint Online, סריקת קורה באופן אוטומטי בהתבסס על לוח הזמנים סריקה המוגדר.</span><span class="sxs-lookup"><span data-stu-id="29cf4-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="29cf4-113">כדי לוודא כי השינויים שלך סריקה, באפשרותך במיוחד [הבקשה יצירת אינדקס מחדש עבור הרשימה או הספריה](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="29cf4-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="29cf4-114">לקבלת סקירה מלאה של סכימת החיפוש, ראה [מבוא סכימת החיפוש](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="29cf4-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


