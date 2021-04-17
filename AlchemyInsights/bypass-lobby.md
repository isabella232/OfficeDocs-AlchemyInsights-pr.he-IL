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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>שליטה בהגדרות חדר הכניסה וברמת ההשתתפות ב- Teams

אם אתה רוצה לאפשר לכולם, כולל משתמשים בחיוג, משתמשים חיצוניים ואנונימיים, לעקוף **את** חדר הכניסה , השתמש ב- PowerShell כדי לבצע משימה זו. להלן דוגמה לשינוי מדיניות הפגישה הכללית עבור הארגון שלך.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

cmdlet זה דורש כעת את השימוש במודול PowerShell של Skype for Business. כדי להגדיר להשתמש ב- cmdlet זה, עיין [בניהול מדיניות באמצעות PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

לאחר הגדרת מדיניות, עליך להחיל אותה על משתמשים; לחלופין, אם שינית את המדיניות הכללית, היא תחול באופן אוטומטי על משתמשים. עבור כל שינוי מדיניות, עליך **להמתין לפחות 4 שעות עד 24 שעות** כדי שהמדיניות תיתוקף. 

הקפד לסקור את התיעוד שלהלן לפני ביצוע שינויים אלה כדי להבין בדיוק מה הדבר מאפשר.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>הכרת פקדי מדיניות חדר הכניסה של פגישת Teams

הגדרות אלה לקבוע אילו משתתפים בפגישה להמתין בחדר הכניסה לפני שהם יתאשפזו בפגישה ואת רמת ההשתתפות שהם מורשים בפגישה. באפשרותך להשתמש ב- PowerShell כדי לעדכן הגדרות מדיניות פגישה שעדיין לא יושמו (עם תווית "בקרוב") במרכז הניהול של Teams. ראה להלן cmdlet PowerShell לדוגמה המאפשר לכל המשתמשים לעקוף את חדר הכניסה.

- [קבלה אוטומטית של אנשים](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) היא מדיניות לפי מארגן ה קובעת אם אנשים מצטרפים לפגישה ישירות או להמתין בחדר הכניסה עד שהם יתאשפזו על-ידי משתמש מאומת.

- [אפשר לאנשים אנונימיים](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) להתחיל פגישה היא מדיניות לפי מארגן ה קובעת אם אנשים אנונימיים, כולל B2B ומשתמשים מאוחדים, יכולים להצטרף לפגישה של המשתמש ללא משתמש מאומת מהארגון הנוכחי.

- [אפשר למשתמשי](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) חיוג נכנס לעקוף את חדר הכניסה **(** בקרוב) היא מדיניות לפי מארגן הקובעת אם אנשים שמתחייגים באמצעות הטלפון מצטרפים לפגישה ישירות או להמתין בחדר הכניסה ללא קשר **להגדרה 'קבלה אוטומטית של אנשים'.**

- [אפשר למארגנים](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) לעקוף את הגדרות חדר הכניסה (בקרוב) היא מדיניות לפי מארגן שקבעה אם  מארגן  הפגישה יכול לעקוף את הגדרות חדר הכניסה שקבע מנהל מערכת ב' הכניסה באופן אוטומטי לאנשים ולאפשר למשתמשים בחיוג לעקוף את חדר הכניסה כאשר הם מתזמן פגישה חדשה.

**הערה:** קרא [את ניהול מדיניות הפגישה ב- Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) לקבלת מבט כולל על מדיניות הפגישה של Microsoft Teams.
