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
# <a name="control-lobby-settings-and-level-of-participation"></a>שליטה בהגדרות הלובי וברמת ההשתתפות

אם ברצונך לאפשר לכולם, כולל חיוג, משתמשים חיצוניים ואנונימיים לעקוף את הלובי, באפשרותך להשתמש ב-PowerShell כדי לעשות זאת. להלן דוגמה לשינוי מדיניות הפגישה הגלובלית עבור הארגון שלך:

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

יישומון זה כרגע דורש שימוש במודול סקייפ לעסק PowerShell. כדי לגרום לתוכנית ההתקנה להשתמש ב-cmdlet זה, עיין בניהול מדיניות באמצעות PowerShell.

באפשרותך להגדיר מדיניות חדשה, שבה יהיה עליך להחיל אותה על משתמשים. אם תשנה את המדיניות הכללית, היא תחול באופן אוטומטי על משתמשים. עבור כל שינוי מדיניות, עליך להמתין לפחות 4 שעות עד 24 שעות כדי שהמדיניות ייכנסו לתוקף.

הקפד לסקור את התיעוד שלהלן לפני ביצוע שינויים אלה כדי להבין בדיוק מה הדבר מאפשר.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>הבנת קבוצות של פקדי מדיניות לובי

- [להודות באופן אוטומטי שאנשים](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) היא מדיניות לפי מארגן הקובעת אם אנשים יצטרפו לפגישה ישירות או יחכו בלובי עד שהם יאוודו על-ידי משתמש מאומת.

- [אפשר לאנשים אנונימיים להתחיל פגישה](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) היא מדיניות לפי מארגן הקובעת אם אנשים אנונימיים, לרבות B2B ומשתמשים מאוחדים, יכולים להצטרף לפגישה של המשתמש ללא משתמש מאומת מהארגון בנוכחות.

- [אפשר למשתמשי חיוג לעקוף את הלובי](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**בקרוב**) היא מדיניות לפי מארגן השולטת אם אנשים המשתמשים בחיוג באמצעות הטלפון מצטרפים ישירות לפגישה או ממתינים בלובי ללא קשר להגדרת **האנשים שבאופן אוטומטי** .

- [אפשר למארגנים לעקוף את הגדרות הלובי](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**בקרוב**) היא מדיניות לפי מארגן הקובעת אם מארגן הפגישה יכול לעקוף את הגדרות הלובי שערכת מנהל **באופן אוטומטי מודה לאנשים** **ולאפשר חיוג נכנס משתמשים לעקוף את הלובי** כאשר הם מזמנים פגישה חדשה.

**הערה:** קרא [ניהול מדיניות פגישה בצוותים](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) לקבלת סקירה מלאה של מדיניות הפגישות של צוותי Microsoft.
