---
title: ויסות מקוונות של SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931443"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="cb520-102">ויסות מקוונות של SharePoint</span><span class="sxs-lookup"><span data-stu-id="cb520-102">SharePoint Online throttling</span></span>

<span data-ttu-id="cb520-103">**חשוב**: לקוחות רבים של SharePoint Online ו-onedrive מנהלים יישומים קריטיים לעסקים נגד השירות המנוהל ברקע.</span><span class="sxs-lookup"><span data-stu-id="cb520-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="cb520-104">אלה כוללים העברת תוכן, מניעת אובדן נתונים (DLP) ופתרונות גיבוי.</span><span class="sxs-lookup"><span data-stu-id="cb520-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="cb520-105">במהלך זמנים חסרי תקדים אלה, אנו נוטלים צעדים כדי להבטיח ששירותי SharePoint Online ו-OneDrive יישארו זמינים ואמינים עבור המשתמשים התלויים בשירות יותר מתמיד בתרחישי עבודה מרוחקים.</span><span class="sxs-lookup"><span data-stu-id="cb520-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="cb520-106">לתמיכה במטרה זו, אנו הטמיעה מגבלות ויסות הדוק יותר על יישומי הרקע (הגירה, DLP ופתרונות גיבוי) בשעות היום של ימי חול.</span><span class="sxs-lookup"><span data-stu-id="cb520-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="cb520-107">אתה צריך לצפות כי יישומים אלה להשיג תפוקה מוגבלת מאוד במהלך הזמנים האלה.</span><span class="sxs-lookup"><span data-stu-id="cb520-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="cb520-108">עם זאת, בשעות הערב ובסוף השבוע של האזור, השירות יהיה מוכן לעבד נפח גבוה יותר באופן משמעותי של בקשות מיישומי רקע.</span><span class="sxs-lookup"><span data-stu-id="cb520-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="cb520-109">**ויסות מקוונות של SharePoint**</span><span class="sxs-lookup"><span data-stu-id="cb520-109">**SharePoint Online throttling**</span></span>

<span data-ttu-id="cb520-110">SharePoint Online משתמש בוויסות כדי לשמור על ביצועים ואמינות אופטימליים של שירות SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="cb520-110">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="cb520-111">האפשרות ' ויסות ' מגבילה את מספר פעולות המשתמש או שיחות בו (לפי סקריפט או קוד) כדי למנוע שימוש יתר במשאבים.</span><span class="sxs-lookup"><span data-stu-id="cb520-111">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="cb520-112">למידע נוסף, אנא בקרו בקישורים שלהלן.</span><span class="sxs-lookup"><span data-stu-id="cb520-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="cb520-113">הימנע מקבלת נחנקו או חסום ב-SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="cb520-113">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="cb520-114">העברת נתונים ויסות SPO</span><span class="sxs-lookup"><span data-stu-id="cb520-114">Data Migration and SPO Throttling </span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [<span data-ttu-id="cb520-115">SharePoint Online ו-OneDrive מהירות הגירה</span><span class="sxs-lookup"><span data-stu-id="cb520-115">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [<span data-ttu-id="cb520-116">טיפול בוויסות מקוון של SharePoint באמצעות חזרה מעריכית</span><span class="sxs-lookup"><span data-stu-id="cb520-116">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [<span data-ttu-id="cb520-117">תכנון קיבולת ובדיקת עומס של SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="cb520-117">Capacity planning and load testing SharePoint Online</span></span>](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

