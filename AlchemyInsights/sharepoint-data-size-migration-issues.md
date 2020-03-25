---
title: בעיות בעת העברת נתונים ל-SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "1885"
ms.openlocfilehash: b53a98480bab48497274c7358f7e606caa477f5a
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931695"
---
# <a name="issues-while-migrating-data-to-sharepoint-online"></a><span data-ttu-id="2cd44-102">בעיות בעת העברת נתונים ל-SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="2cd44-102">Issues while migrating data to SharePoint Online</span></span>

<span data-ttu-id="2cd44-103">**חשוב**: לקוחות רבים של SharePoint Online ו-onedrive מנהלים יישומים קריטיים לעסקים נגד השירות המנוהל ברקע.</span><span class="sxs-lookup"><span data-stu-id="2cd44-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="2cd44-104">אלה כוללים העברת תוכן, מניעת אובדן נתונים (DLP) ופתרונות גיבוי.</span><span class="sxs-lookup"><span data-stu-id="2cd44-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="2cd44-105">במהלך זמנים חסרי תקדים אלה, אנו נוטלים צעדים כדי להבטיח ששירותי SharePoint Online ו-OneDrive יישארו זמינים ואמינים עבור המשתמשים התלויים בשירות יותר מתמיד בתרחישי עבודה מרוחקים.</span><span class="sxs-lookup"><span data-stu-id="2cd44-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="2cd44-106">לתמיכה במטרה זו, אנו הטמיעה מגבלות ויסות הדוק יותר על יישומי הרקע (הגירה, DLP ופתרונות גיבוי) בשעות היום של ימי חול.</span><span class="sxs-lookup"><span data-stu-id="2cd44-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="2cd44-107">אתה צריך לצפות כי יישומים אלה להשיג תפוקה מוגבלת מאוד במהלך הזמנים האלה.</span><span class="sxs-lookup"><span data-stu-id="2cd44-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="2cd44-108">עם זאת, בשעות הערב ובסוף השבוע של האזור, השירות יהיה מוכן לעבד נפח גבוה יותר באופן משמעותי של בקשות מיישומי רקע.</span><span class="sxs-lookup"><span data-stu-id="2cd44-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="2cd44-109">**מעביר מעל 100 טרה-בתים של נתונים**</span><span class="sxs-lookup"><span data-stu-id="2cd44-109">**Migrating over 100TB of data**</span></span>

<span data-ttu-id="2cd44-110">נראה שאתה מעביר מעל 100TB של נתונים ל-SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="2cd44-110">It appears you are migrating over 100TB of data to SharePoint Online.</span></span> <span data-ttu-id="2cd44-111">נא בצע את השלבים הבאים כדי שנוכל לסייע לך בהקדם האפשרי.</span><span class="sxs-lookup"><span data-stu-id="2cd44-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="2cd44-112">בחר **בקשת שירות חדשה**ולאחר מכן **בקשת שירות חדשה**.</span><span class="sxs-lookup"><span data-stu-id="2cd44-112">Select **New Service Request**, and then **New Service Request**.</span></span> 
2. <span data-ttu-id="2cd44-113">השאר את הכותרת והתיאור **כהעברת SharePoint מעל 100 טרה-בתים**.</span><span class="sxs-lookup"><span data-stu-id="2cd44-113">Leave the title and description as **SharePoint migration over 100TB**.</span></span>
3. <span data-ttu-id="2cd44-114">לאחר הגשת הכרטיס, אנא עדכנו אותו במידע הבא:</span><span class="sxs-lookup"><span data-stu-id="2cd44-114">Once the ticket has been submitted, please update it with the following information:</span></span> 

    - <span data-ttu-id="2cd44-115">הגודל המשוער של ההעברה.</span><span class="sxs-lookup"><span data-stu-id="2cd44-115">Estimated size of your migration.</span></span>
    - <span data-ttu-id="2cd44-116">הערכה של מתי ברצונך להתחיל ולהשלים את ההעברה.</span><span class="sxs-lookup"><span data-stu-id="2cd44-116">An estimate of when you would like to start and complete your migration.</span></span>
    - <span data-ttu-id="2cd44-117">תאר היכן אתה מעביר את התוכן שלך, כגון SharePoint Server, Box, GDrive, שיתופי קבצים וכו '.</span><span class="sxs-lookup"><span data-stu-id="2cd44-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>


  

