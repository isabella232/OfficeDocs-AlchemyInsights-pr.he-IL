---
title: לובי מעקף
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684951"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="91a0e-102">שליטה בהגדרות הלובי וברמת ההשתתפות ב-Teams</span><span class="sxs-lookup"><span data-stu-id="91a0e-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="91a0e-103">אם ברצונך לאפשר לכולם, כולל משתמשים בחיוג, משתמשים חיצוניים ואנונימיים, **לעקוף את הכניסה, השתמש**ב-PowerShell כדי לבצע משימה זו.</span><span class="sxs-lookup"><span data-stu-id="91a0e-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="91a0e-104">להלן דוגמה של שינוי מדיניות הפגישה הכללית עבור הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="91a0e-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="91a0e-105">רכיב cmdlet זה מחייב כעת את השימוש במודול מודול PowerShell של Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="91a0e-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="91a0e-106">כדי להגדיר כדי להשתמש ב-cmdlet זה, עיין [בניהול מדיניות באמצעות PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="91a0e-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="91a0e-107">לאחר הגדרת מדיניות, עליך להחיל אותה על משתמשים; לחלופין, אם שינית את המדיניות הכללית, היא תחול באופן אוטומטי על משתמשים.</span><span class="sxs-lookup"><span data-stu-id="91a0e-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="91a0e-108">עבור כל שינוי מדיניות, עליך להמתין לפחות **4 שעות עד 24 שעות עד** שמדיניות המדיניות תיכנס לתוקף.</span><span class="sxs-lookup"><span data-stu-id="91a0e-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="91a0e-109">הקפד לסקור את התיעוד שלהלן לפני ביצוע שינויים אלה כדי להבין בדיוק מה הדבר מאפשר.</span><span class="sxs-lookup"><span data-stu-id="91a0e-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="91a0e-110">הכרת פקדי מדיניות לובי הפגישה של Teams</span><span class="sxs-lookup"><span data-stu-id="91a0e-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="91a0e-111">הגדרות אלה קובעות אילו משתתפי הפגישה יחכו בחדר הכניסה לפני שיתקבלו לפגישה ולרמת ההשתתפות שהם מותרים בפגישה.</span><span class="sxs-lookup"><span data-stu-id="91a0e-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="91a0e-112">באפשרותך להשתמש ב-PowerShell כדי לעדכן את הגדרות מדיניות הפגישה שעדיין לא יושמה (המסומנות באות "בקרוב") במרכז הניהול של Teams.</span><span class="sxs-lookup"><span data-stu-id="91a0e-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="91a0e-113">ראה להלן רכיב cmdlet של PowerShell לדוגמה המאפשר לכל המשתמשים לעקוף את חדר הכניסה.</span><span class="sxs-lookup"><span data-stu-id="91a0e-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="91a0e-114">[מודה באופן אוטומטי שאנשים](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) היא מדיניות לכל מארגן הקובעת אם אנשים מצטרפים לפגישה ישירות או ממתינים בחדר הכניסה עד שמשתמש מאומת יתקבל.</span><span class="sxs-lookup"><span data-stu-id="91a0e-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="91a0e-115">[אפשר לאנשים אנונימיים להתחיל פגישה](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) היא מדיניות לכל מארגן שקובעת אם אנשים אנונימיים, כולל B2B ומשתמשים מאוחדים, יכולים להצטרף לפגישת המשתמש ללא משתמש מאומת מהארגון בנוכחות.</span><span class="sxs-lookup"><span data-stu-id="91a0e-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="91a0e-116">[אפשר למשתמשי חיוג לעקוף את חדר הכניסה](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**בקרוב**) היא מדיניות לכל מארגן שקובעת אם אנשים המחייגים באמצעות הטלפון מצטרפים לפגישה ישירות או ממתינים בחדר הכניסה ללא קשר להגדרת **האנשים המתודיים באופן אוטומטי** .</span><span class="sxs-lookup"><span data-stu-id="91a0e-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="91a0e-117">[אפשר למארגנים לעקוף הגדרות לובי](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**בקרוב**) היא מדיניות לכל מארגן שקובעת אם מארגן הפגישה יכול לעקוף את הגדרות הכניסה שמנהל מערכת **מודה באופן אוטומטי על אנשים** **ולאפשר למשתמשי חיוג לעקוף את הכניסה** בעת תזמון פגישה חדשה.</span><span class="sxs-lookup"><span data-stu-id="91a0e-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="91a0e-118">**הערה:** קרא [לנהל מדיניות פגישה ב-teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) לקבלת סקירה מלאה של מדיניות הפגישה של Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="91a0e-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
