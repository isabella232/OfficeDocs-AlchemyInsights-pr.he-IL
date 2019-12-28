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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>שליטה בהגדרות הלובי וברמת ההשתתפות בצוותים

אם ברצונך לאפשר לכולם, כולל חיוג, משתמשים חיצוניים ואנונימיים, **לעקוף את הלובי**, השתמש ב-PowerShell כדי לבצע משימה זו. להלן דוגמה לשינוי מדיניות הפגישה הגלובלית עבור הארגון שלך.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

יישומון זה כרגע דורש שימוש במודול סקייפ לעסק PowerShell. כדי לקבל הגדרת כדי להשתמש ב-cmdlet זה, הוצאת [ניהול מדיניות באמצעות PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

לאחר הגדרת מדיניות, עליך להחילו על משתמשים; לחלופין, אם שינית את המדיניות הכללית, היא תחול באופן אוטומטי על משתמשים. עבור שינוי מדיניות כלשהו, עליך להמתין לפחות **4 שעות עד 24 שעות** כדי שפריטי המדיניות ייכנסו לתוקף. 

הקפד לסקור את התיעוד שלהלן לפני ביצוע שינויים אלה כדי להבין בדיוק מה הדבר מאפשר.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>הבנת קבוצות של פקדי מדיניות לובי

הגדרות אלה קובעות באיזו פגישה המשתתפים ממתינים בלובי לפני שהם מגיעים לפגישה ולרמת ההשתתפות הם מותרים בפגישה. באפשרותך להשתמש ב-PowerShell כדי לעדכן הגדרות מדיניות פגישה שעדיין לא יושמו (המסומנות כ"בקרוב בקרוב") במרכז הניהול של הצוותים. ראה להלן לדוגמה PowerShell cmdlet המאפשר לכל המשתמשים לעקוף את הלובי.

- [להודות באופן אוטומטי שאנשים](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) היא מדיניות לפי מארגן הקובעת אם אנשים יצטרפו לפגישה ישירות או יחכו בלובי עד שהם יאוודו על-ידי משתמש מאומת.

- [אפשר לאנשים אנונימיים להתחיל פגישה](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) היא מדיניות לפי מארגן הקובעת אם אנשים אנונימיים, לרבות B2B ומשתמשים מאוחדים, יכולים להצטרף לפגישה של המשתמש ללא משתמש מאומת מהארגון בנוכחות.

- [אפשר למשתמשי חיוג לעקוף את הלובי](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**בקרוב**) היא מדיניות לפי מארגן השולטת אם אנשים המשתמשים בחיוג באמצעות הטלפון מצטרפים ישירות לפגישה או ממתינים בלובי ללא קשר להגדרת **האנשים שבאופן אוטומטי** .

- [אפשר למארגנים לעקוף את הגדרות הלובי](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**בקרוב**) היא מדיניות לפי מארגן הקובעת אם מארגן הפגישה יכול לעקוף את הגדרות הלובי שערכת מנהל **באופן אוטומטי מודה לאנשים** **ולאפשר למשתמשי חיוג לעקוף את הלובי** כאשר הם מזמנים פגישה חדשה.

**הערה:** קרא [ניהול מדיניות פגישה בצוותים](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) לקבלת סקירה מלאה של מדיניות הפגישות של צוותי Microsoft.
