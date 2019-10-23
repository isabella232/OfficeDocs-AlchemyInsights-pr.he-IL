---
title: לובי מעקפים
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 729fc5d4213acbbdf74a9d07adacb42b34170717
ms.sourcegitcommit: ffbeb72c9199ab4ebcb0f1ad443ed3e2f4950efc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/23/2019
ms.locfileid: "37637778"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="16af5-102">שליטה בהגדרות הלובי וברמת ההשתתפות</span><span class="sxs-lookup"><span data-stu-id="16af5-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="16af5-103">אם ברצונך לאפשר לכולם, כולל חיוג, משתמשים חיצוניים ואנונימיים לעקוף את הלובי, באפשרותך להשתמש ב-PowerShell כדי לעשות זאת.</span><span class="sxs-lookup"><span data-stu-id="16af5-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby, you can use PowerShell to do it.</span></span> <span data-ttu-id="16af5-104">להלן דוגמה לשינוי מדיניות הפגישה הגלובלית עבור הארגון שלך:</span><span class="sxs-lookup"><span data-stu-id="16af5-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="16af5-105">יישומון זה כרגע דורש שימוש במודול סקייפ לעסק PowerShell.</span><span class="sxs-lookup"><span data-stu-id="16af5-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="16af5-106">כדי לגרום לתוכנית ההתקנה להשתמש ב-cmdlet זה, עיין בניהול מדיניות באמצעות PowerShell.</span><span class="sxs-lookup"><span data-stu-id="16af5-106">To get setup to use this cmdlet, check out Managing policies via PowerShell.</span></span>

<span data-ttu-id="16af5-107">באפשרותך להגדיר מדיניות חדשה, שבה יהיה עליך להחיל אותה על משתמשים.</span><span class="sxs-lookup"><span data-stu-id="16af5-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="16af5-108">אם תשנה את המדיניות הכללית, היא תחול באופן אוטומטי על משתמשים.</span><span class="sxs-lookup"><span data-stu-id="16af5-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="16af5-109">עבור כל שינוי מדיניות, עליך להמתין לפחות 4 שעות עד 24 שעות כדי שהמדיניות ייכנסו לתוקף.</span><span class="sxs-lookup"><span data-stu-id="16af5-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="16af5-110">הקפד לסקור את התיעוד שלהלן לפני ביצוע שינויים אלה כדי להבין בדיוק מה הדבר מאפשר.</span><span class="sxs-lookup"><span data-stu-id="16af5-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="16af5-111">הבנת קבוצות של פקדי מדיניות לובי</span><span class="sxs-lookup"><span data-stu-id="16af5-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="16af5-112">[להודות באופן אוטומטי שאנשים](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) היא מדיניות לפי מארגן הקובעת אם אנשים יצטרפו לפגישה ישירות או יחכו בלובי עד שהם יאוודו על-ידי משתמש מאומת.</span><span class="sxs-lookup"><span data-stu-id="16af5-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="16af5-113">[אפשר לאנשים אנונימיים להתחיל פגישה](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) היא מדיניות לפי מארגן הקובעת אם אנשים אנונימיים, לרבות B2B ומשתמשים מאוחדים, יכולים להצטרף לפגישה של המשתמש ללא משתמש מאומת מהארגון בנוכחות.</span><span class="sxs-lookup"><span data-stu-id="16af5-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="16af5-114">[אפשר למשתמשי חיוג לעקוף את הלובי](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**בקרוב**) היא מדיניות לפי מארגן השולטת אם אנשים המשתמשים בחיוג באמצעות הטלפון מצטרפים ישירות לפגישה או ממתינים בלובי ללא קשר להגדרת **האנשים שבאופן אוטומטי** .</span><span class="sxs-lookup"><span data-stu-id="16af5-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="16af5-115">[אפשר למארגנים לעקוף את הגדרות הלובי](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**בקרוב**) היא מדיניות לפי מארגן הקובעת אם מארגן הפגישה יכול לעקוף את הגדרות הלובי שערכת מנהל **באופן אוטומטי מודה לאנשים** **ולאפשר חיוג נכנס משתמשים לעקוף את הלובי** כאשר הם מזמנים פגישה חדשה.</span><span class="sxs-lookup"><span data-stu-id="16af5-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="16af5-116">**הערה:** קרא [ניהול מדיניות פגישה בצוותים](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) לקבלת סקירה מלאה של מדיניות הפגישות של צוותי Microsoft.</span><span class="sxs-lookup"><span data-stu-id="16af5-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
