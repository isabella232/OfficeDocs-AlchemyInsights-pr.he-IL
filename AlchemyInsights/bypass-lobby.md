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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>שליטה בהגדרות הלובי וברמת ההשתתפות ב-Teams

אם ברצונך לאפשר לכולם, כולל משתמשים בחיוג, משתמשים חיצוניים ואנונימיים, **לעקוף את הכניסה, השתמש**ב-PowerShell כדי לבצע משימה זו. להלן דוגמה של שינוי מדיניות הפגישה הכללית עבור הארגון שלך.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

רכיב cmdlet זה מחייב כעת את השימוש במודול מודול PowerShell של Skype for Business. כדי להגדיר כדי להשתמש ב-cmdlet זה, עיין [בניהול מדיניות באמצעות PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

לאחר הגדרת מדיניות, עליך להחיל אותה על משתמשים; לחלופין, אם שינית את המדיניות הכללית, היא תחול באופן אוטומטי על משתמשים. עבור כל שינוי מדיניות, עליך להמתין לפחות **4 שעות עד 24 שעות עד** שמדיניות המדיניות תיכנס לתוקף. 

הקפד לסקור את התיעוד שלהלן לפני ביצוע שינויים אלה כדי להבין בדיוק מה הדבר מאפשר.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>הכרת פקדי מדיניות לובי הפגישה של Teams

הגדרות אלה קובעות אילו משתתפי הפגישה יחכו בחדר הכניסה לפני שיתקבלו לפגישה ולרמת ההשתתפות שהם מותרים בפגישה. באפשרותך להשתמש ב-PowerShell כדי לעדכן את הגדרות מדיניות הפגישה שעדיין לא יושמה (המסומנות באות "בקרוב") במרכז הניהול של Teams. ראה להלן רכיב cmdlet של PowerShell לדוגמה המאפשר לכל המשתמשים לעקוף את חדר הכניסה.

- [מודה באופן אוטומטי שאנשים](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) היא מדיניות לכל מארגן הקובעת אם אנשים מצטרפים לפגישה ישירות או ממתינים בחדר הכניסה עד שמשתמש מאומת יתקבל.

- [אפשר לאנשים אנונימיים להתחיל פגישה](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) היא מדיניות לכל מארגן שקובעת אם אנשים אנונימיים, כולל B2B ומשתמשים מאוחדים, יכולים להצטרף לפגישת המשתמש ללא משתמש מאומת מהארגון בנוכחות.

- [אפשר למשתמשי חיוג לעקוף את חדר הכניסה](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**בקרוב**) היא מדיניות לכל מארגן שקובעת אם אנשים המחייגים באמצעות הטלפון מצטרפים לפגישה ישירות או ממתינים בחדר הכניסה ללא קשר להגדרת **האנשים המתודיים באופן אוטומטי** .

- [אפשר למארגנים לעקוף הגדרות לובי](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**בקרוב**) היא מדיניות לכל מארגן שקובעת אם מארגן הפגישה יכול לעקוף את הגדרות הכניסה שמנהל מערכת **מודה באופן אוטומטי על אנשים** **ולאפשר למשתמשי חיוג לעקוף את הכניסה** בעת תזמון פגישה חדשה.

**הערה:** קרא [לנהל מדיניות פגישה ב-teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) לקבלת סקירה מלאה של מדיניות הפגישה של Microsoft teams.
