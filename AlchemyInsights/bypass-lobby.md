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
ms.openlocfilehash: bf8be9ffe2bfa45ed2cf149c1c4fa118b40e816d
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768441"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="4c94e-102">שליטה בהגדרות הלובי וברמת ההשתתפות</span><span class="sxs-lookup"><span data-stu-id="4c94e-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="4c94e-103">אם ברצונך לאפשר לכולם, כולל חיוג, משתמשים חיצוניים ואנונימיים לעקוף את הלובי בצוותי Microsoft, באפשרותך להשתמש ב-PowerShell כדי לעשות זאת.</span><span class="sxs-lookup"><span data-stu-id="4c94e-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users to bypass the lobby in Microsoft Teams, you can use PowerShell to do it.</span></span> <span data-ttu-id="4c94e-104">להלן דוגמה לשינוי מדיניות הפגישה הגלובלית עבור הארגון שלך:</span><span class="sxs-lookup"><span data-stu-id="4c94e-104">Here's an example of modifying the global meeting policy for your organization:</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="4c94e-105">יישומון זה כרגע דורש שימוש במודול סקייפ לעסק PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4c94e-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="4c94e-106">כדי לקבל את תוכנית ההתקנה להשתמש ב-cmdlet זה, הוצאת [ניהול מדיניות באמצעות PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="4c94e-106">To get setup to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="4c94e-107">באפשרותך להגדיר מדיניות חדשה, שבה יהיה עליך להחיל אותה על משתמשים.</span><span class="sxs-lookup"><span data-stu-id="4c94e-107">You can set up a new policy, which you'll then need to apply it to users.</span></span> <span data-ttu-id="4c94e-108">אם תשנה את המדיניות הכללית, היא תחול באופן אוטומטי על משתמשים.</span><span class="sxs-lookup"><span data-stu-id="4c94e-108">If you modify the Global policy it'll automatically apply to users.</span></span> <span data-ttu-id="4c94e-109">עבור כל שינוי מדיניות, עליך להמתין לפחות 4 שעות עד 24 שעות כדי שהמדיניות ייכנסו לתוקף.</span><span class="sxs-lookup"><span data-stu-id="4c94e-109">For any policy change you need to wait at least 4 hours and up to 24 hours for the policies to take effect.</span></span>

<span data-ttu-id="4c94e-110">הקפד לסקור את התיעוד שלהלן לפני ביצוע שינויים אלה כדי להבין בדיוק מה הדבר מאפשר.</span><span class="sxs-lookup"><span data-stu-id="4c94e-110">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>

## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="4c94e-111">הבנת קבוצות של פקדי מדיניות לובי</span><span class="sxs-lookup"><span data-stu-id="4c94e-111">Understanding Teams meeting lobby policy controls</span></span>

- <span data-ttu-id="4c94e-112">[להודות באופן אוטומטי שאנשים](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) היא מדיניות לפי מארגן הקובעת אם אנשים יצטרפו לפגישה ישירות או יחכו בלובי עד שהם יאוודו על-ידי משתמש מאומת.</span><span class="sxs-lookup"><span data-stu-id="4c94e-112">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="4c94e-113">[אפשר לאנשים אנונימיים להתחיל פגישה](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) היא מדיניות לפי מארגן הקובעת אם אנשים אנונימיים, לרבות B2B ומשתמשים מאוחדים, יכולים להצטרף לפגישה של המשתמש ללא משתמש מאומת מהארגון בנוכחות.</span><span class="sxs-lookup"><span data-stu-id="4c94e-113">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="4c94e-114">[אפשר למשתמשי חיוג לעקוף את הלובי](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**בקרוב**) היא מדיניות לפי מארגן השולטת אם אנשים המשתמשים בחיוג באמצעות הטלפון מצטרפים ישירות לפגישה או ממתינים בלובי ללא קשר להגדרת **האנשים שבאופן אוטומטי** .</span><span class="sxs-lookup"><span data-stu-id="4c94e-114">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="4c94e-115">[אפשר למארגנים לעקוף את הגדרות הלובי](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**בקרוב**) היא מדיניות לפי מארגן הקובעת אם מארגן הפגישה יכול לעקוף את הגדרות הלובי שערכת מנהל **באופן אוטומטי מודה לאנשים** **ולאפשר למשתמשי חיוג לעקוף את הלובי** כאשר הם מזמנים פגישה חדשה.</span><span class="sxs-lookup"><span data-stu-id="4c94e-115">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="4c94e-116">**הערה:** קרא [ניהול מדיניות פגישה בצוותים](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) לקבלת סקירה מלאה של מדיניות הפגישות של צוותי Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4c94e-116">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
