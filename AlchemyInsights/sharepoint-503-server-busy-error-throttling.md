---
title: ויסות מקוונות של SharePoint
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931227"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="37b9c-102">ויסות מקוונות של SharePoint</span><span class="sxs-lookup"><span data-stu-id="37b9c-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="37b9c-103">**חשוב**: לקוחות רבים של SharePoint Online ו-onedrive מנהלים יישומים קריטיים לעסקים נגד השירות המנוהל ברקע.</span><span class="sxs-lookup"><span data-stu-id="37b9c-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="37b9c-104">אלה כוללים העברת תוכן, מניעת אובדן נתונים (DLP) ופתרונות גיבוי.</span><span class="sxs-lookup"><span data-stu-id="37b9c-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="37b9c-105">במהלך זמנים חסרי תקדים אלה, אנו נוטלים צעדים כדי להבטיח ששירותי SharePoint Online ו-OneDrive יישארו זמינים ואמינים עבור המשתמשים התלויים בשירות יותר מתמיד בתרחישי עבודה מרוחקים.</span><span class="sxs-lookup"><span data-stu-id="37b9c-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="37b9c-106">לתמיכה במטרה זו, אנו הטמיעה מגבלות ויסות הדוק יותר על יישומי הרקע (הגירה, DLP ופתרונות גיבוי) בשעות היום של ימי חול.</span><span class="sxs-lookup"><span data-stu-id="37b9c-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="37b9c-107">אתה צריך לצפות כי יישומים אלה להשיג תפוקה מוגבלת מאוד במהלך הזמנים האלה.</span><span class="sxs-lookup"><span data-stu-id="37b9c-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="37b9c-108">עם זאת, בשעות הערב ובסוף השבוע של האזור, השירות יהיה מוכן לעבד נפח גבוה יותר באופן משמעותי של בקשות מיישומי רקע.</span><span class="sxs-lookup"><span data-stu-id="37b9c-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="37b9c-109">**503 שרת הוא שגיאה עמוסה**</span><span class="sxs-lookup"><span data-stu-id="37b9c-109">**503 server is busy error**</span></span>

<span data-ttu-id="37b9c-110">משתמשים עלולים לקבל שרת 503 הוא שגיאה עמוסה בעת ניסיון לנווט אל אתרי SharePoint או OneDrive.</span><span class="sxs-lookup"><span data-stu-id="37b9c-110">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="37b9c-111">שגיאה זו עשויה להיגרם על-ידי ויסות בתוך שירות SharePoint.</span><span class="sxs-lookup"><span data-stu-id="37b9c-111">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="37b9c-112">SharePoint Online משתמש בוויסות כדי לשמור על ביצועים ואמינות אופטימליים של שירות SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="37b9c-112">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="37b9c-113">האפשרות ' ויסות ' מגבילה את מספר פעולות המשתמש או שיחות בו (לפי סקריפט או קוד) כדי למנוע שימוש יתר במשאבים.</span><span class="sxs-lookup"><span data-stu-id="37b9c-113">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="37b9c-114">לקבלת מידע נוסף על ויסות לראות, [הימנע מקבלת נחנקו או חסום ב-SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="37b9c-114">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="37b9c-115">אם אתה סבור ששגיאה זו אינה קשורה לוויסות, באפשרותך לבדוק אם קיים תחזוקה פעילה המתרחשת בדייר שלך על-ידי ניווט [למרכז ההודעות](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="37b9c-115">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="37b9c-116">לבסוף, ודא שאתה מבקר בדף [הבריאות של השירות](https://portal.office.com/adminportal/home#/servicehealth) כדי לבדוק אם יש עלוני יידוע/אירועים שעשויים להתרחש.</span><span class="sxs-lookup"><span data-stu-id="37b9c-116">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

