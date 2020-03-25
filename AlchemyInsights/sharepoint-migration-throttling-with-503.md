---
title: ויסות העברה של SharePoint עם 503 שגיאות
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931659"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="cab67-102">ויסות העברה של SharePoint עם 503 שגיאות</span><span class="sxs-lookup"><span data-stu-id="cab67-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="cab67-103">**חשוב**: לקוחות רבים של SharePoint Online ו-onedrive מנהלים יישומים קריטיים לעסקים נגד השירות המנוהל ברקע.</span><span class="sxs-lookup"><span data-stu-id="cab67-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="cab67-104">אלה כוללים העברת תוכן, מניעת אובדן נתונים (DLP) ופתרונות גיבוי.</span><span class="sxs-lookup"><span data-stu-id="cab67-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="cab67-105">במהלך זמנים חסרי תקדים אלה, אנו נוטלים צעדים כדי להבטיח ששירותי SharePoint Online ו-OneDrive יישארו זמינים ואמינים עבור המשתמשים התלויים בשירות יותר מתמיד בתרחישי עבודה מרוחקים.</span><span class="sxs-lookup"><span data-stu-id="cab67-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="cab67-106">לתמיכה במטרה זו, אנו הטמיעה מגבלות ויסות הדוק יותר על יישומי הרקע (הגירה, DLP ופתרונות גיבוי) בשעות היום של ימי חול.</span><span class="sxs-lookup"><span data-stu-id="cab67-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="cab67-107">אתה צריך לצפות כי יישומים אלה להשיג תפוקה מוגבלת מאוד במהלך הזמנים האלה.</span><span class="sxs-lookup"><span data-stu-id="cab67-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="cab67-108">עם זאת, בשעות הערב ובסוף השבוע של האזור, השירות יהיה מוכן לעבד נפח גבוה יותר באופן משמעותי של בקשות מיישומי רקע.</span><span class="sxs-lookup"><span data-stu-id="cab67-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="cab67-109">**503 שגיאות בעת הגירה ל-SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="cab67-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="cab67-110">נראה שאתה מעביר ל-SharePoint Online ומקבל 503 שגיאות.</span><span class="sxs-lookup"><span data-stu-id="cab67-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="cab67-111">נא בצע את השלבים הבאים כדי שנוכל לסייע לך בהקדם האפשרי.</span><span class="sxs-lookup"><span data-stu-id="cab67-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="cab67-112">לחץ על **תמיכה באנשי קשר**ולאחר מכן **בקשת שירות חדשה**.</span><span class="sxs-lookup"><span data-stu-id="cab67-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="cab67-113">עבור הכותרת והתיאור, הקלד **ויסות העברת SharePoint עם 503**.</span><span class="sxs-lookup"><span data-stu-id="cab67-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="cab67-114">לאחר הגשת הכרטיס, אנא עדכנו אותו במידע הבא:</span><span class="sxs-lookup"><span data-stu-id="cab67-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="cab67-115">כמה משמאל של הגירה (לדוגמה, כמה TBs?).</span><span class="sxs-lookup"><span data-stu-id="cab67-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="cab67-116">תאריך התחלה וסיום של העברה.</span><span class="sxs-lookup"><span data-stu-id="cab67-116">Migration start and end date.</span></span>
    - <span data-ttu-id="cab67-117">תאר היכן אתה מעביר את התוכן שלך, כגון SharePoint Server, Box, GDrive, שיתופי קבצים וכו '.</span><span class="sxs-lookup"><span data-stu-id="cab67-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="cab67-118">האם להעריך את מספר שגיאות הוויסות (לדוגמה, x המצערת לשעה?) ומתי הוויסות יתרחש.</span><span class="sxs-lookup"><span data-stu-id="cab67-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="cab67-119">באיזה כלי הגירה אתה משתמש (לדוגמה, SPMT או ShareGate).</span><span class="sxs-lookup"><span data-stu-id="cab67-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


