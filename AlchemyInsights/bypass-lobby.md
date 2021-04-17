---
title: עקיפת חדר הכניסה
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820035"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="aa3eb-102">שליטה בהגדרות חדר הכניסה וברמת ההשתתפות ב- Teams</span><span class="sxs-lookup"><span data-stu-id="aa3eb-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="aa3eb-103">אם אתה רוצה לאפשר לכולם, כולל משתמשים בחיוג, משתמשים חיצוניים ואנונימיים, לעקוף **את** חדר הכניסה , השתמש ב- PowerShell כדי לבצע משימה זו.</span><span class="sxs-lookup"><span data-stu-id="aa3eb-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="aa3eb-104">להלן דוגמה לשינוי מדיניות הפגישה הכללית עבור הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="aa3eb-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="aa3eb-105">cmdlet זה דורש כעת את השימוש במודול PowerShell של Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="aa3eb-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="aa3eb-106">כדי להגדיר להשתמש ב- cmdlet זה, עיין [בניהול מדיניות באמצעות PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="aa3eb-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="aa3eb-107">לאחר הגדרת מדיניות, עליך להחיל אותה על משתמשים; לחלופין, אם שינית את המדיניות הכללית, היא תחול באופן אוטומטי על משתמשים.</span><span class="sxs-lookup"><span data-stu-id="aa3eb-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="aa3eb-108">עבור כל שינוי מדיניות, עליך **להמתין לפחות 4 שעות עד 24 שעות** כדי שהמדיניות תיתוקף.</span><span class="sxs-lookup"><span data-stu-id="aa3eb-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="aa3eb-109">הקפד לסקור את התיעוד שלהלן לפני ביצוע שינויים אלה כדי להבין בדיוק מה הדבר מאפשר.</span><span class="sxs-lookup"><span data-stu-id="aa3eb-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="aa3eb-110">הכרת פקדי מדיניות חדר הכניסה של פגישת Teams</span><span class="sxs-lookup"><span data-stu-id="aa3eb-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="aa3eb-111">הגדרות אלה לקבוע אילו משתתפים בפגישה להמתין בחדר הכניסה לפני שהם יתאשפזו בפגישה ואת רמת ההשתתפות שהם מורשים בפגישה.</span><span class="sxs-lookup"><span data-stu-id="aa3eb-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="aa3eb-112">באפשרותך להשתמש ב- PowerShell כדי לעדכן הגדרות מדיניות פגישה שעדיין לא יושמו (עם תווית "בקרוב") במרכז הניהול של Teams.</span><span class="sxs-lookup"><span data-stu-id="aa3eb-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="aa3eb-113">ראה להלן cmdlet PowerShell לדוגמה המאפשר לכל המשתמשים לעקוף את חדר הכניסה.</span><span class="sxs-lookup"><span data-stu-id="aa3eb-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="aa3eb-114">[קבלה אוטומטית של אנשים](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) היא מדיניות לפי מארגן ה קובעת אם אנשים מצטרפים לפגישה ישירות או להמתין בחדר הכניסה עד שהם יתאשפזו על-ידי משתמש מאומת.</span><span class="sxs-lookup"><span data-stu-id="aa3eb-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="aa3eb-115">[אפשר לאנשים אנונימיים](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) להתחיל פגישה היא מדיניות לפי מארגן ה קובעת אם אנשים אנונימיים, כולל B2B ומשתמשים מאוחדים, יכולים להצטרף לפגישה של המשתמש ללא משתמש מאומת מהארגון הנוכחי.</span><span class="sxs-lookup"><span data-stu-id="aa3eb-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="aa3eb-116">[אפשר למשתמשי](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) חיוג נכנס לעקוף את חדר הכניסה **(** בקרוב) היא מדיניות לפי מארגן הקובעת אם אנשים שמתחייגים באמצעות הטלפון מצטרפים לפגישה ישירות או להמתין בחדר הכניסה ללא קשר **להגדרה 'קבלה אוטומטית של אנשים'.**</span><span class="sxs-lookup"><span data-stu-id="aa3eb-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="aa3eb-117">[אפשר למארגנים](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) לעקוף את הגדרות חדר הכניסה (בקרוב) היא מדיניות לפי מארגן שקבעה אם  מארגן  הפגישה יכול לעקוף את הגדרות חדר הכניסה שקבע מנהל מערכת ב' הכניסה באופן אוטומטי לאנשים ולאפשר למשתמשים בחיוג לעקוף את חדר הכניסה כאשר הם מתזמן פגישה חדשה.</span><span class="sxs-lookup"><span data-stu-id="aa3eb-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="aa3eb-118">**הערה:** קרא [את ניהול מדיניות הפגישה ב- Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) לקבלת מבט כולל על מדיניות הפגישה של Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="aa3eb-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
