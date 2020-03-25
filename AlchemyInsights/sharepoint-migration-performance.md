---
title: ביצועי העברה של SharePoint
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
- "2700"
ms.openlocfilehash: 812444589d5a5bf766bbc6f466077d4ca829d79f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932236"
---
# <a name="sharepoint-migration-performance"></a><span data-ttu-id="a52cd-102">ביצועי העברה של SharePoint</span><span class="sxs-lookup"><span data-stu-id="a52cd-102">SharePoint migration performance</span></span>

<span data-ttu-id="a52cd-103">**חשוב**: לקוחות SharePoint Online ו- OneDrive רבים מפעילים אפליקציות חיוניות לעסקים בניגוד לשירות שפועל ברקע.</span><span class="sxs-lookup"><span data-stu-id="a52cd-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="a52cd-104">אפליקציות אלו כוללות העברת תוכן, מניעת אובדן נתונים (DLP) ופתרונות גיבוי.</span><span class="sxs-lookup"><span data-stu-id="a52cd-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="a52cd-105">במהלך תקופה חסרת תקדים זו, אנחנו נוקטים בצעדים כדי שישמרו על הזמינות הגבוהה והאמינות של שירות SharePoint Online ו- OneDrive עבור המשתמשים שלך אשר תלויים בשירות יותר מאי פעם בתרחישי עבודה מרחוק.</span><span class="sxs-lookup"><span data-stu-id="a52cd-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="a52cd-106">כחלק מהתמיכה במטרה זו, יישמנו מגבלות ויסות הדוקות יותר על יישומי רקע (העברה, DLP ופתרונות רקע) במהלך שעות העבודה בימי חול.</span><span class="sxs-lookup"><span data-stu-id="a52cd-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="a52cd-107">אתה יכול לצפות לתפוקה מוגבלת מאוד של יישומים אלה במועדים אלה.</span><span class="sxs-lookup"><span data-stu-id="a52cd-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="a52cd-108">אולם, בשעות הערב ובסופי שבוע באזור, השירות יהיה מוכן לעבד נפח גבוה באופן משמעותי של בקשות מיישומי רקע.</span><span class="sxs-lookup"><span data-stu-id="a52cd-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="a52cd-109">**ביצועי העברה**</span><span class="sxs-lookup"><span data-stu-id="a52cd-109">**Migration performance**</span></span>

<span data-ttu-id="a52cd-110">ניתן להשפיע על ביצועי העברה על-ידי תשתיות רשת, גודל קובץ, זמן ההעברה וויסותו.</span><span class="sxs-lookup"><span data-stu-id="a52cd-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="a52cd-111">הבנה של גורמים אלו יכולה לעשות לך לתכנן ולמקסם את היעילות של ההעברה שלך.</span><span class="sxs-lookup"><span data-stu-id="a52cd-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

<span data-ttu-id="a52cd-112">לקבלת פרטים נוספים, בקר בקישורים שלהלן.</span><span class="sxs-lookup"><span data-stu-id="a52cd-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="a52cd-113">Sharepoint Online ומהירות העברה של ODB</span><span class="sxs-lookup"><span data-stu-id="a52cd-113">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="a52cd-114">הימנעות מוויסות או חסימה ב- SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="a52cd-114">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="a52cd-115">הורדה והתקנה של כלי ההעברה של SharePoint</span><span class="sxs-lookup"><span data-stu-id="a52cd-115">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
