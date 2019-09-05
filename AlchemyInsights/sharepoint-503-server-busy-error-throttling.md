---
title: ויסות מקוונות של SharePoint
ms.author: pebaum
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: d9e1400697b1e6435fea78703d2ecadc6733a57f
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751889"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="56c9b-102">ויסות מקוונות של SharePoint</span><span class="sxs-lookup"><span data-stu-id="56c9b-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="56c9b-103">משתמשים עלולים לקבל שרת 503 הוא שגיאה עמוסה בעת ניסיון לנווט אל אתרי SharePoint או OneDrive.</span><span class="sxs-lookup"><span data-stu-id="56c9b-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="56c9b-104">שגיאה זו עשויה להיגרם על-ידי ויסות בתוך שירות SharePoint.</span><span class="sxs-lookup"><span data-stu-id="56c9b-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="56c9b-105">SharePoint Online משתמש בוויסות כדי לשמור על ביצועים ואמינות אופטימליים של שירות SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="56c9b-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="56c9b-106">האפשרות ' ויסות ' מגבילה את מספר פעולות המשתמש או שיחות בו (לפי סקריפט או קוד) כדי למנוע שימוש יתר במשאבים.</span><span class="sxs-lookup"><span data-stu-id="56c9b-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="56c9b-107">אם אתה מקבל נחנקו, 99% מהזמן הוא בגלל קוד מותאם אישית.</span><span class="sxs-lookup"><span data-stu-id="56c9b-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="56c9b-108">לקבלת מידע נוסף על ויסות לראות, [הימנע מקבלת נחנקו או חסום ב-SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="56c9b-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="56c9b-109">אם אתה סבור ששגיאה זו אינה קשורה לוויסות, באפשרותך לבדוק אם קיים תחזוקה פעילה המתרחשת בדייר שלך על-ידי ניווט [למרכז ההודעות](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="56c9b-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="56c9b-110">לבסוף, ודא שאתה מבקר בדף [הבריאות של השירות](https://portal.office.com/adminportal/home#/servicehealth) כדי לבדוק אם יש עלוני יידוע/אירועים שעשויים להתרחש.</span><span class="sxs-lookup"><span data-stu-id="56c9b-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

