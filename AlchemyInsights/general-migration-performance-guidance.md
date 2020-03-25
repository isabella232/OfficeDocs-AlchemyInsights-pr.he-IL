---
title: הדרכה כללית של ביצועי ההעברה
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3179"
ms.openlocfilehash: 10a0069c41d2e5128b2592425d815364a83b730f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932480"
---
# <a name="general-migration-performance-guidance"></a><span data-ttu-id="5c824-102">הדרכה כללית של ביצועי ההעברה</span><span class="sxs-lookup"><span data-stu-id="5c824-102">General migration performance guidance</span></span>

<span data-ttu-id="5c824-103">**חשוב**: לקוחות SharePoint Online ו- OneDrive רבים מפעילים אפליקציות חיוניות לעסקים בניגוד לשירות שפועל ברקע.</span><span class="sxs-lookup"><span data-stu-id="5c824-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="5c824-104">אפליקציות אלו כוללות העברת תוכן, מניעת אובדן נתונים (DLP) ופתרונות גיבוי.</span><span class="sxs-lookup"><span data-stu-id="5c824-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="5c824-105">במהלך תקופה חסרת תקדים זו, אנחנו נוקטים בצעדים כדי שישמרו על הזמינות הגבוהה והאמינות של שירות SharePoint Online ו- OneDrive עבור המשתמשים שלך אשר תלויים בשירות יותר מאי פעם בתרחישי עבודה מרחוק.</span><span class="sxs-lookup"><span data-stu-id="5c824-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="5c824-106">כחלק מהתמיכה במטרה זו, יישמנו מגבלות ויסות הדוקות יותר על יישומי רקע (העברה, DLP ופתרונות רקע) במהלך שעות העבודה בימי חול.</span><span class="sxs-lookup"><span data-stu-id="5c824-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="5c824-107">אתה יכול לצפות לתפוקה מוגבלת מאוד של יישומים אלה במועדים אלה.</span><span class="sxs-lookup"><span data-stu-id="5c824-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="5c824-108">אולם, בשעות הערב ובסופי שבוע באזור, השירות יהיה מוכן לעבד נפח גבוה באופן משמעותי של בקשות מיישומי רקע.</span><span class="sxs-lookup"><span data-stu-id="5c824-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="5c824-109">**הדרכה של ביצועי העברה**</span><span class="sxs-lookup"><span data-stu-id="5c824-109">**Migration performance guidance**</span></span>

<span data-ttu-id="5c824-110">ניתן להשפיע על ביצועי העברה על-ידי תשתיות רשת, גודל קובץ, זמן ההעברה וויסותו.</span><span class="sxs-lookup"><span data-stu-id="5c824-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="5c824-111">הבנה של גורמים אלו יכולה לעשות לך לתכנן ולמקסם את היעילות של ההעברה שלך.</span><span class="sxs-lookup"><span data-stu-id="5c824-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

- [<span data-ttu-id="5c824-112">הדרכה כללית של ביצועי העברה</span><span class="sxs-lookup"><span data-stu-id="5c824-112">General migration performance guidance</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
