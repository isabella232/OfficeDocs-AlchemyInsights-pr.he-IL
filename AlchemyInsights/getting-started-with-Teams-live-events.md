---
title: תחילת העבודה עם אירועים בשידור חי של Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000208"
- "3436"
ms.openlocfilehash: a10f756fc69a7a135446d8d3bcec1f5e951627d8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811961"
---
# <a name="getting-started-with-teams-live-events"></a><span data-ttu-id="8cba1-102">תחילת העבודה עם אירועים בשידור חי של Teams</span><span class="sxs-lookup"><span data-stu-id="8cba1-102">Getting started with Teams live events</span></span>

<span data-ttu-id="8cba1-103">אירועים בשידור חי של Microsoft Teams הם החרבה של פגישות Teams שמאפשרים לך לקבוע מועד של אירועים ולהפיק אירועים שזורמים לקבל מקוון גדול.</span><span class="sxs-lookup"><span data-stu-id="8cba1-103">Microsoft Teams live events are an extension of Teams meetings that enable you to schedule and produce events that stream to large online audiences.</span></span>

<span data-ttu-id="8cba1-104">כדי ליצור אירוע בשידור חי, תצטרך את הדברים הבאים:</span><span class="sxs-lookup"><span data-stu-id="8cba1-104">To create a live event, you will need the following:</span></span>

- <span data-ttu-id="8cba1-105">תחילה, אשר שאירועי Teams Live [זמינים במדינה ובאזור שלך;](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability) אירועים בשידור חי אינם נתמכים עדיין במדינות מסוימות.</span><span class="sxs-lookup"><span data-stu-id="8cba1-105">First, confirm that Teams Live Events are [available in your Country and Region](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Live Events are not yet supported in some countries.</span></span>  <span data-ttu-id="8cba1-106">אם הקצהת רשיונות וקבעת פריטי מדיניות, אך עדיין אינך מצליח ליצור אירוע Teams Live, סביר מאוד שאתה נמצא במדינה או באזור שבו אירועים בשידור חי עדיין אינם זמינים.</span><span class="sxs-lookup"><span data-stu-id="8cba1-106">If you’ve assigned licenses and set policies, but still cannot create a Teams Live Event, it is likely you are in a Country or Region where Live Events is not yet available.</span></span>

- <span data-ttu-id="8cba1-107">רישיון [Office 365 Enterprise E1, E3, או E5 או רישיון Office 365 A3 או רישיון A5](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="8cba1-107">An [Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span></span> <span data-ttu-id="8cba1-108">**הערה**: עקב שימוש מוגבר ב- Teams לאחרונה, כאשר אתה מקצה למשתמש רישיון Teams, ייתכן שיחלפו 24 שעות לפני שהוא יוגדר במלואו.</span><span class="sxs-lookup"><span data-stu-id="8cba1-108">**Note**: Due to a recent increase in Teams usage, when you assign a Teams license to a user, it may take around 24 hours before they'll be fully set up.</span></span> <span data-ttu-id="8cba1-109">עד אז, לא תוכל להקצות להם פריטי מדיניות של Teams, וייתכן שלא תהיה להם גישה לתכונות מסוימות של Teams, כגון ועידות שמע.</span><span class="sxs-lookup"><span data-stu-id="8cba1-109">Until then, you won't be able to assign Teams policies to them, and they might not have access to some Teams features like calling and audio conferencing.</span></span>

- <span data-ttu-id="8cba1-110">הרשאה כדי [ליצור אירועים בשידור חי במרכז הניהול של Microsoft Teams](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span><span class="sxs-lookup"><span data-stu-id="8cba1-110">Permission to [create live events in Microsoft Teams admin center](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span></span>

- <span data-ttu-id="8cba1-111">הרשאה כדי [ליצור אירועים בשידור חי ב- Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (עבור אירועים שמופקים באמצעות יישום או מכשיר שידור חיצוני).</span><span class="sxs-lookup"><span data-stu-id="8cba1-111">Permission to [create live events in Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (for events produced using an external broadcasting app or device).</span></span>

- <span data-ttu-id="8cba1-112">חברות צוות מלאה בארגון (אינך יכול להיות אורח או מארגון אחר)</span><span class="sxs-lookup"><span data-stu-id="8cba1-112">Full team membership in the org (can't be a guest or from another org).</span></span>
<span data-ttu-id="8cba1-113">האפשרויות קביעת מועד פגישה פרטית, שיתוף מסך ושיתוף IP וידאו צריכות להיות מופעלות במדיניות פגישת צוות.</span><span class="sxs-lookup"><span data-stu-id="8cba1-113">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

- <span data-ttu-id="8cba1-114">[שיטות עבודה מומלצות](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) עבור אירועים בשידור חי ב- Teams.</span><span class="sxs-lookup"><span data-stu-id="8cba1-114">[Best practices](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) for Teams Live Events.</span></span>

<span data-ttu-id="8cba1-115">לקבלת מידע נוסף, ראה [התחל לעבוד עם אירועים בשידור חי של Microsoft Teams](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span><span class="sxs-lookup"><span data-stu-id="8cba1-115">For more information, please see [Get started with Microsoft Teams live events](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span></span>