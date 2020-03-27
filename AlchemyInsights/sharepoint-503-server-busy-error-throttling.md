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
ms.openlocfilehash: 2aca55ac2fefbb2035140a759a77730dc905a4e9
ms.sourcegitcommit: 926e4ab6aa64ddc7a244de633421eb2b817541f2
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/26/2020
ms.locfileid: "42958722"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="b4da4-102">ויסות מקוונות של SharePoint</span><span class="sxs-lookup"><span data-stu-id="b4da4-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="b4da4-103">**חשוב**: במהלך הזמנים חסרי התקדים האלה, אנו נוטלים צעדים כדי להבטיח ששירותי sharepoint online ו-onedrive יישארו זמינים במידה רבה – אנא בקר [בהתאמות התכונות הזמניות של sharepoint online](https://aka.ms/ODSPAdjustments) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="b4da4-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="b4da4-104">**503 שרת הוא שגיאה עמוסה**</span><span class="sxs-lookup"><span data-stu-id="b4da4-104">**503 server is busy error**</span></span>

<span data-ttu-id="b4da4-105">משתמשים עלולים לקבל שרת 503 הוא שגיאה עמוסה בעת ניסיון לנווט אל אתרי SharePoint או OneDrive.</span><span class="sxs-lookup"><span data-stu-id="b4da4-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="b4da4-106">שגיאה זו עשויה להיגרם על-ידי ויסות בתוך שירות SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b4da4-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="b4da4-107">SharePoint Online משתמש בוויסות כדי לשמור על ביצועים ואמינות אופטימליים של שירות SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="b4da4-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="b4da4-108">האפשרות ' ויסות ' מגבילה את מספר פעולות המשתמש או שיחות בו (לפי סקריפט או קוד) כדי למנוע שימוש יתר במשאבים.</span><span class="sxs-lookup"><span data-stu-id="b4da4-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="b4da4-109">לקבלת מידע נוסף על ויסות לראות, [הימנע מקבלת נחנקו או חסום ב-SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="b4da4-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="b4da4-110">אם אתה סבור ששגיאה זו אינה קשורה לוויסות, באפשרותך לבדוק אם קיים תחזוקה פעילה המתרחשת בדייר שלך על-ידי ניווט [למרכז ההודעות](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="b4da4-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="b4da4-111">לבסוף, ודא שאתה מבקר בדף [הבריאות של השירות](https://portal.office.com/adminportal/home#/servicehealth) כדי לבדוק אם יש עלוני יידוע/אירועים שעשויים להתרחש.</span><span class="sxs-lookup"><span data-stu-id="b4da4-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

