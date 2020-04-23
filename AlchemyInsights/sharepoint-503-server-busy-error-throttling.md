---
title: ויסות מקוונות של SharePoint
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 50b2c29db1fd294abe6c9e60f067156109de392b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742210"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="4d00f-102">ויסות מקוונות של SharePoint</span><span class="sxs-lookup"><span data-stu-id="4d00f-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="4d00f-103">**חשוב**: בתקופה חסרת תקדים זאת, אנחנו נוקטים בצעדים כדי להבטיח ששירותי SharePoint Online ו- OneDrive יישארו בזמינות גבוהה - לקבלת מידע נוסף, בקר בכתובת[התאמות של תכונה זמנית ב- SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="4d00f-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="4d00f-104">**503 שרת הוא שגיאה עמוסה**</span><span class="sxs-lookup"><span data-stu-id="4d00f-104">**503 server is busy error**</span></span>

<span data-ttu-id="4d00f-105">משתמשים עלולים לקבל שרת 503 הוא שגיאה עמוסה בעת ניסיון לנווט אל אתרי SharePoint או OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4d00f-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="4d00f-106">שגיאה זו עשויה להיגרם על-ידי ויסות בתוך שירות SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4d00f-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="4d00f-107">SharePoint Online משתמש בוויסות כדי לשמור על ביצועים ומהימנות אופטימליים של שירות SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="4d00f-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="4d00f-108">ויסות מגביל את מספר פעולות המשתמש או מספר השיחות בו-זמנית (לפי script או קוד) כדי למנוע שימוש מופרז במשאבים.</span><span class="sxs-lookup"><span data-stu-id="4d00f-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="4d00f-109">לקבלת מידע נוסף על ויסות לראות, [הימנע מקבלת נחנקו או חסום ב-SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="4d00f-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="4d00f-110">אם אתה סבור ששגיאה זו אינה קשורה לוויסות, באפשרותך לבדוק אם קיים תחזוקה פעילה המתרחשת בדייר שלך על-ידי ניווט [למרכז ההודעות](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="4d00f-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="4d00f-111">לבסוף, ודא שאתה מבקר בדף [הבריאות של השירות](https://portal.office.com/adminportal/home#/servicehealth) כדי לבדוק אם יש עלוני יידוע/אירועים שעשויים להתרחש.</span><span class="sxs-lookup"><span data-stu-id="4d00f-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

