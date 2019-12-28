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
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889083"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="af539-102">שליטה בהגדרות הלובי וברמת ההשתתפות בצוותים</span><span class="sxs-lookup"><span data-stu-id="af539-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="af539-103">אם ברצונך לאפשר לכולם, כולל חיוג, משתמשים חיצוניים ואנונימיים, **לעקוף את הלובי**, השתמש ב-PowerShell כדי לבצע משימה זו.</span><span class="sxs-lookup"><span data-stu-id="af539-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="af539-104">להלן דוגמה לשינוי מדיניות הפגישה הגלובלית עבור הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="af539-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="af539-105">יישומון זה כרגע דורש שימוש במודול סקייפ לעסק PowerShell.</span><span class="sxs-lookup"><span data-stu-id="af539-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="af539-106">כדי לקבל הגדרת כדי להשתמש ב-cmdlet זה, הוצאת [ניהול מדיניות באמצעות PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="af539-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="af539-107">לאחר הגדרת מדיניות, עליך להחילו על משתמשים; לחלופין, אם שינית את המדיניות הכללית, היא תחול באופן אוטומטי על משתמשים.</span><span class="sxs-lookup"><span data-stu-id="af539-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="af539-108">עבור שינוי מדיניות כלשהו, עליך להמתין לפחות **4 שעות עד 24 שעות** כדי שפריטי המדיניות ייכנסו לתוקף.</span><span class="sxs-lookup"><span data-stu-id="af539-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="af539-109">הקפד לסקור את התיעוד שלהלן לפני ביצוע שינויים אלה כדי להבין בדיוק מה הדבר מאפשר.</span><span class="sxs-lookup"><span data-stu-id="af539-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="af539-110">הבנת קבוצות של פקדי מדיניות לובי</span><span class="sxs-lookup"><span data-stu-id="af539-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="af539-111">הגדרות אלה קובעות באיזו פגישה המשתתפים ממתינים בלובי לפני שהם מגיעים לפגישה ולרמת ההשתתפות הם מותרים בפגישה.</span><span class="sxs-lookup"><span data-stu-id="af539-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="af539-112">באפשרותך להשתמש ב-PowerShell כדי לעדכן הגדרות מדיניות פגישה שעדיין לא יושמו (המסומנות כ"בקרוב בקרוב") במרכז הניהול של הצוותים.</span><span class="sxs-lookup"><span data-stu-id="af539-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="af539-113">ראה להלן לדוגמה PowerShell cmdlet המאפשר לכל המשתמשים לעקוף את הלובי.</span><span class="sxs-lookup"><span data-stu-id="af539-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="af539-114">[להודות באופן אוטומטי שאנשים](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) היא מדיניות לפי מארגן הקובעת אם אנשים יצטרפו לפגישה ישירות או יחכו בלובי עד שהם יאוודו על-ידי משתמש מאומת.</span><span class="sxs-lookup"><span data-stu-id="af539-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="af539-115">[אפשר לאנשים אנונימיים להתחיל פגישה](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) היא מדיניות לפי מארגן הקובעת אם אנשים אנונימיים, לרבות B2B ומשתמשים מאוחדים, יכולים להצטרף לפגישה של המשתמש ללא משתמש מאומת מהארגון בנוכחות.</span><span class="sxs-lookup"><span data-stu-id="af539-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="af539-116">[אפשר למשתמשי חיוג לעקוף את הלובי](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**בקרוב**) היא מדיניות לפי מארגן השולטת אם אנשים המשתמשים בחיוג באמצעות הטלפון מצטרפים ישירות לפגישה או ממתינים בלובי ללא קשר להגדרת **האנשים שבאופן אוטומטי** .</span><span class="sxs-lookup"><span data-stu-id="af539-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="af539-117">[אפשר למארגנים לעקוף את הגדרות הלובי](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**בקרוב**) היא מדיניות לפי מארגן הקובעת אם מארגן הפגישה יכול לעקוף את הגדרות הלובי שערכת מנהל **באופן אוטומטי מודה לאנשים** **ולאפשר למשתמשי חיוג לעקוף את הלובי** כאשר הם מזמנים פגישה חדשה.</span><span class="sxs-lookup"><span data-stu-id="af539-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="af539-118">**הערה:** קרא [ניהול מדיניות פגישה בצוותים](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) לקבלת סקירה מלאה של מדיניות הפגישות של צוותי Microsoft.</span><span class="sxs-lookup"><span data-stu-id="af539-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
