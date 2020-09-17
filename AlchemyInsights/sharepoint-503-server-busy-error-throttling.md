---
title: ויסות SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 21d0f8d0118d92562b425921742513157563b5fb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773848"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="68c21-102">ויסות SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="68c21-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="68c21-103">**חשוב**: בתקופה חסרת תקדים זאת, אנחנו נוקטים בצעדים כדי להבטיח ששירותי SharePoint Online ו- OneDrive יישארו בזמינות גבוהה - לקבלת מידע נוסף, בקר בכתובת[התאמות של תכונה זמנית ב- SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="68c21-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="68c21-104">**שגיאה של 503 server עמוסה**</span><span class="sxs-lookup"><span data-stu-id="68c21-104">**503 server is busy error**</span></span>

<span data-ttu-id="68c21-105">משתמשים עשויים לקבל שגיאה של 503 server עמוסה בעת ניסיון לנווט לאתרי SharePoint או OneDrive.</span><span class="sxs-lookup"><span data-stu-id="68c21-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="68c21-106">שגיאה זו עשויה להיגרם כתוצאה מוויסות בשירות SharePoint.</span><span class="sxs-lookup"><span data-stu-id="68c21-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="68c21-107">SharePoint Online משתמש בוויסות כדי לשמור על ביצועים ומהימנות אופטימליים של שירות SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="68c21-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="68c21-108">ויסות מגביל את מספר פעולות המשתמש או מספר השיחות בו-זמנית (לפי script או קוד) כדי למנוע שימוש מופרז במשאבים.</span><span class="sxs-lookup"><span data-stu-id="68c21-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="68c21-109">לקבלת מידע נוסף אודות ויסות, ראה [הימנעות מקבלת מצערת או חסומה ב-SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="68c21-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="68c21-110">אם אתה סבור ששגיאה זו אינה קשורה לוויסות, באפשרותך לבדוק אם יש תחזוקה פעילה שמתרחשת בדייר שלך על-ידי ניווט [למרכז ההודעות](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="68c21-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="68c21-111">לבסוף, ודא שאתה מבקר בדף [תקינות השירות](https://portal.office.com/adminportal/home#/servicehealth) כדי לבדוק את כל העלונים/האירועים שעשויים להתרחש.</span><span class="sxs-lookup"><span data-stu-id="68c21-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

