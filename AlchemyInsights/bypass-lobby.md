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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376669"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="3152a-102">שליטה בהגדרות הלובי וברמת ההשתתפות</span><span class="sxs-lookup"><span data-stu-id="3152a-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="3152a-103">הגדרות אלה קובעות באיזו פגישה המשתתפים ממתינים בלובי לפני שהם מגיעים לפגישה ולרמת ההשתתפות הם מותרים בפגישה.</span><span class="sxs-lookup"><span data-stu-id="3152a-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="3152a-104">באפשרותך להשתמש ב-Powershell כדי לעדכן הגדרות מדיניות פגישה שטרם יושמו (המסומנות כ"בקרוב בקרוב") במרכז המנהלים של הצוותים.</span><span class="sxs-lookup"><span data-stu-id="3152a-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="3152a-105">ראה להלן לדוגמה PowerShell cmdlet המאפשר לכל המשתמשים לעקוף את הלובי.</span><span class="sxs-lookup"><span data-stu-id="3152a-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="3152a-106">[להודות באופן אוטומטי שאנשים](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) היא מדיניות לפי מארגן הקובעת אם אנשים יצטרפו לפגישה ישירות או יחכו בלובי עד שהם יאוודו על-ידי משתמש מאומת.</span><span class="sxs-lookup"><span data-stu-id="3152a-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="3152a-107">[אפשר לאנשים אנונימיים להתחיל פגישה](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) היא מדיניות לפי מארגן הקובעת אם אנשים אנונימיים, לרבות B2B ומשתמשים מאוחדים, יכולים להצטרף לפגישה של המשתמש ללא משתמש מאומת מהארגון בנוכחות.</span><span class="sxs-lookup"><span data-stu-id="3152a-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="3152a-108">[אפשר למשתמשי חיוג לעקוף את הלובי](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**בקרוב**) היא מדיניות לפי מארגן השולטת אם אנשים המשתמשים בחיוג באמצעות הטלפון מצטרפים ישירות לפגישה או ממתינים בלובי ללא קשר להגדרת **האנשים שבאופן אוטומטי** .</span><span class="sxs-lookup"><span data-stu-id="3152a-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="3152a-109">[אפשר למארגנים לעקוף את הגדרות הלובי](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**בקרוב**) היא מדיניות לפי מארגן הקובעת אם מארגן הפגישה יכול לעקוף את הגדרות הלובי שערכת מנהל **באופן אוטומטי מודה לאנשים** **ולאפשר חיוג נכנס משתמשים לעקוף את הלובי** כאשר הם מזמנים פגישה חדשה.</span><span class="sxs-lookup"><span data-stu-id="3152a-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="3152a-110">**הערה:** קרא [ניהול מדיניות פגישה בצוותים](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) לקבלת סקירה מלאה של מדיניות הפגישות של צוותי Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3152a-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="3152a-111">**ממשל PowerShell**</span><span class="sxs-lookup"><span data-stu-id="3152a-111">**PowerShell example**</span></span>

<span data-ttu-id="3152a-112">אם ברצונך לאפשר לכולם, כולל משתמשים חיצוניים או אנונימיים, לעקוף את הלובי, באפשרותך גם להשתמש ב-PowerShell כדי לבצע משימה זו.</span><span class="sxs-lookup"><span data-stu-id="3152a-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="3152a-113">להלן דוגמה לשינוי מדיניות הפגישה הגלובלית עבור הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="3152a-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="3152a-114">(הקפד לסקור את התיעוד לעיל לפני ביצוע שינויים אלה כדי להבין בדיוק מה זה מאפשר.)</span><span class="sxs-lookup"><span data-stu-id="3152a-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="3152a-115">סט מדיניות-הAllowPSTNUsersToBypassLobby הכללית של זהות המשתמש "כולם"-מ$True</span><span class="sxs-lookup"><span data-stu-id="3152a-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="3152a-116">לקבלת מידע נוסף, ראה [הגדרת מדיניות מוגדרת](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="3152a-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>
