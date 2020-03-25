---
title: העברת אפשרויות ל-SharePoint Online
ms.author: pebaum
author: v-miegge
manager: v-cojank
ms.date: 11/04/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: c8c339c9-2e50-4daa-aa91-3eb5053e2bc6
ms.openlocfilehash: 830b39c51658cbc02f4be81acdfdf3b164a8df70
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932731"
---
# <a name="migrate-options-to-sharepoint-online"></a><span data-ttu-id="e4692-102">העברת אפשרויות ל-SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="e4692-102">Migrate options to SharePoint Online</span></span>

<span data-ttu-id="e4692-103">**חשוב**: לקוחות רבים של SharePoint Online ו-onedrive מנהלים יישומים קריטיים לעסקים נגד השירות המנוהל ברקע.</span><span class="sxs-lookup"><span data-stu-id="e4692-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="e4692-104">אלה כוללים העברת תוכן, מניעת אובדן נתונים (DLP) ופתרונות גיבוי.</span><span class="sxs-lookup"><span data-stu-id="e4692-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="e4692-105">במהלך זמנים חסרי תקדים אלה, אנו נוטלים צעדים כדי להבטיח ששירותי SharePoint Online ו-OneDrive יישארו זמינים ואמינים עבור המשתמשים התלויים בשירות יותר מתמיד בתרחישי עבודה מרוחקים.</span><span class="sxs-lookup"><span data-stu-id="e4692-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="e4692-106">לתמיכה במטרה זו, אנו הטמיעה מגבלות ויסות הדוק יותר על יישומי הרקע (הגירה, DLP ופתרונות גיבוי) בשעות היום של ימי חול.</span><span class="sxs-lookup"><span data-stu-id="e4692-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="e4692-107">אתה צריך לצפות כי יישומים אלה להשיג תפוקה מוגבלת מאוד במהלך הזמנים האלה.</span><span class="sxs-lookup"><span data-stu-id="e4692-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="e4692-108">עם זאת, בשעות הערב ובסוף השבוע של האזור, השירות יהיה מוכן לעבד נפח גבוה יותר באופן משמעותי של בקשות מיישומי רקע.</span><span class="sxs-lookup"><span data-stu-id="e4692-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="e4692-109">**אפשרויות הגירה**</span><span class="sxs-lookup"><span data-stu-id="e4692-109">**Migration options**</span></span>

<span data-ttu-id="e4692-110">קיימות אפשרויות שונות הזמינות להעברת תוכן ל-SharePoint Online, בהתאם לגודל ולכמות הקבצים שעליך להעביר, עיין ברשימת האפשרויות [הממוקמות כאן](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="e4692-110">There are different options available to migrate content to SharePoint Online, depending on the size and quantity of files you need to move, please see a list of options [located here](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span></span>

<span data-ttu-id="e4692-111">לקבלת מידע נוסף אודות העברת תוכן, בקר בקישורים שלהלן.</span><span class="sxs-lookup"><span data-stu-id="e4692-111">For more information on content migration, please visit the links below.</span></span>

- [<span data-ttu-id="e4692-112">כלי להעברת Sharepoint</span><span class="sxs-lookup"><span data-stu-id="e4692-112">Sharepoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)

- [<span data-ttu-id="e4692-113">התחל לעבוד עם מנהל ההעברות</span><span class="sxs-lookup"><span data-stu-id="e4692-113">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="e4692-114">מהירות העברה של Sharepoint Online ו-ODB</span><span class="sxs-lookup"><span data-stu-id="e4692-114">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="e4692-115">הימנע מקבלת נחנקו או חסום ב-SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="e4692-115">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="e4692-116">כלי להערכת הגירה של SharePoint (SMAT)</span><span class="sxs-lookup"><span data-stu-id="e4692-116">SharePoint Migration Assessment Tool (SMAT)</span></span>](https://www.microsoft.com/download/details.aspx?id=53598&amp;751be11f-ede8-5a0c-058c-2ee190a24fa6=True)

<span data-ttu-id="e4692-117">**הערה**: כרגע הכלי להעברת SharePoint תומך רק בהעברות מ-SharePoint 2010 ו-2013.</span><span class="sxs-lookup"><span data-stu-id="e4692-117">**Note**: Currently the SharePoint Migration tool only support migrations from SharePoint 2010  and 2013.</span></span> <span data-ttu-id="e4692-118">גירסה 2016 או 2019 אינן נתמכות בשלב זה.</span><span class="sxs-lookup"><span data-stu-id="e4692-118">Version 2016 or 2019 are not supported at this time.</span></span>
