---
title: בעיות ביצועים-SharePoint או OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068404"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="cbd71-102">SharePoint או OneDrive איטי, לא נגיש או לא זמין עבור משתמשים מרובים</span><span class="sxs-lookup"><span data-stu-id="cbd71-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="cbd71-103">SharePoint או OneDrive עשויים להיות איטיים, לא נגישים או לא זמינים, או שהשירות יציג שירות שאינו זמין או 503 שגיאות, ממספר סיבות:</span><span class="sxs-lookup"><span data-stu-id="cbd71-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="cbd71-104">אם אתר SharePoint או OneDrive שלך איטי או מתעכב עבור משתמשים מרובים, ייתכן שקיימת בעיית שירות זמנית שבה משתמשים חווים עיכובים לסירוגין או שגיאות ניווט בעת גישה לאתרי SharePoint או לתוכן OneDrive.</span><span class="sxs-lookup"><span data-stu-id="cbd71-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="cbd71-105">בדוק את [לוח המחוונים של תקינות השירות](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) כדי לבדוק אם הארגון שלך מושפע.</span><span class="sxs-lookup"><span data-stu-id="cbd71-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="cbd71-106">משתמשים עלולים לקבל *שרת 503 הוא* שגיאה עמוסה בעת ניסיון לנווט אל אתרי SharePoint או onedrive.</span><span class="sxs-lookup"><span data-stu-id="cbd71-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="cbd71-107">שגיאה זו עשויה להיגרם על-ידי ויסות בתוך שירות SharePoint.</span><span class="sxs-lookup"><span data-stu-id="cbd71-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="cbd71-108">SharePoint Online משתמש בוויסות כדי לשמור על ביצועים ואמינות אופטימליים של שירות SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="cbd71-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="cbd71-109">האפשרות ' ויסות ' מגבילה את מספר פעולות המשתמש או שיחות בו (לפי סקריפט או קוד) כדי למנוע שימוש יתר במשאבים.</span><span class="sxs-lookup"><span data-stu-id="cbd71-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="cbd71-110">לקבלת מידע נוסף על ויסות לראות, [הימנע מקבלת נחנקו או חסום ב-SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="cbd71-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="cbd71-111">אם אתה נתקל בביצועים איטיים עם אתר או דף SharePoint **קלאסי** או **מודרני** , נצל את [כלי אבחון העמוד](https://aka.ms/perftool) כדי לנתח את הדפים.</span><span class="sxs-lookup"><span data-stu-id="cbd71-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="cbd71-112">אם אתה עדיין נתקל בביצועים איטיים כלליים, עיין במשאבים בחלק התחתון של מאמר זה: [מבוא לכיוונון ביצועים עבור SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="cbd71-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  