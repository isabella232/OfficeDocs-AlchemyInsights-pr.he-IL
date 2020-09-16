---
title: בעיות ביצועים-SharePoint או OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771902"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="98834-102">SharePoint או OneDrive איטיים, לא נגישים או שאינם זמינים עבור משתמשים מרובים</span><span class="sxs-lookup"><span data-stu-id="98834-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="98834-103">SharePoint או OneDrive עשויים להיות איטיים, בלתי נגישים או שאינם זמינים, או עשויים להציג שגיאות שאינן זמינות או 503, מכמה סיבות:</span><span class="sxs-lookup"><span data-stu-id="98834-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="98834-104">אם האתר שלך ב-SharePoint או ב-OneDrive מתעכב או מעוכב עבור משתמשים מרובים, ייתכן שקיימת בעיה זמנית בשירות שבו משתמשים חווים עיכובים רציפים או שגיאות ניווט בעת גישה לאתרי SharePoint או לתוכן OneDrive.</span><span class="sxs-lookup"><span data-stu-id="98834-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="98834-105">בדוק את [לוח המחוונים של תקינות השירות](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) כדי לבדוק אם הארגון שלך מושפע.</span><span class="sxs-lookup"><span data-stu-id="98834-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="98834-106">משתמשים עשויים לקבל שגיאה של *503 server עמוסה* בעת ניסיון לנווט לאתרי SharePoint או OneDrive.</span><span class="sxs-lookup"><span data-stu-id="98834-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="98834-107">שגיאה זו עשויה להיגרם כתוצאה מוויסות בשירות SharePoint.</span><span class="sxs-lookup"><span data-stu-id="98834-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="98834-108">SharePoint Online משתמש בוויסות כדי לשמור על ביצועים ומהימנות אופטימליים של שירות SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="98834-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="98834-109">ויסות מגביל את מספר פעולות המשתמש או מספר השיחות בו-זמנית (לפי script או קוד) כדי למנוע שימוש מופרז במשאבים.</span><span class="sxs-lookup"><span data-stu-id="98834-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="98834-110">לקבלת מידע נוסף אודות ויסות, ראה [הימנעות מקבלת מצערת או חסומה ב-SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="98834-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="98834-111">אם אתה נתקל בביצועים איטיים באמצעות אתר או אתר SharePoint **קלאסי** או **מודרני** , השתמש [בכלי אבחון העמוד](https://aka.ms/perftool) כדי לנתח את העמודים.</span><span class="sxs-lookup"><span data-stu-id="98834-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="98834-112">אם אתה עדיין נתקל בביצועים איטיים כלליים, עיין במשאבים בחלק התחתון של מאמר זה: [מבוא לכוונון ביצועים עבור SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="98834-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  