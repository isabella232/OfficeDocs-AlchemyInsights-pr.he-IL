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
# <a name="control-lobby-settings-and-level-of-participation"></a>שליטה בהגדרות הלובי וברמת ההשתתפות

הגדרות אלה קובעות באיזו פגישה המשתתפים ממתינים בלובי לפני שהם מגיעים לפגישה ולרמת ההשתתפות הם מותרים בפגישה. באפשרותך להשתמש ב-Powershell כדי לעדכן הגדרות מדיניות פגישה שטרם יושמו (המסומנות כ"בקרוב בקרוב") במרכז המנהלים של הצוותים.  ראה להלן לדוגמה PowerShell cmdlet המאפשר לכל המשתמשים לעקוף את הלובי.  

- [להודות באופן אוטומטי שאנשים](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) היא מדיניות לפי מארגן הקובעת אם אנשים יצטרפו לפגישה ישירות או יחכו בלובי עד שהם יאוודו על-ידי משתמש מאומת.

- [אפשר לאנשים אנונימיים להתחיל פגישה](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) היא מדיניות לפי מארגן הקובעת אם אנשים אנונימיים, לרבות B2B ומשתמשים מאוחדים, יכולים להצטרף לפגישה של המשתמש ללא משתמש מאומת מהארגון בנוכחות.

- [אפשר למשתמשי חיוג לעקוף את הלובי](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**בקרוב**) היא מדיניות לפי מארגן השולטת אם אנשים המשתמשים בחיוג באמצעות הטלפון מצטרפים ישירות לפגישה או ממתינים בלובי ללא קשר להגדרת **האנשים שבאופן אוטומטי** .

- [אפשר למארגנים לעקוף את הגדרות הלובי](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**בקרוב**) היא מדיניות לפי מארגן הקובעת אם מארגן הפגישה יכול לעקוף את הגדרות הלובי שערכת מנהל **באופן אוטומטי מודה לאנשים** **ולאפשר חיוג נכנס משתמשים לעקוף את הלובי** כאשר הם מזמנים פגישה חדשה.

**הערה:** קרא [ניהול מדיניות פגישה בצוותים](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) לקבלת סקירה מלאה של מדיניות הפגישות של צוותי Microsoft. 


**ממשל PowerShell**

אם ברצונך לאפשר לכולם, כולל משתמשים חיצוניים או אנונימיים, לעקוף את הלובי, באפשרותך גם להשתמש ב-PowerShell כדי לבצע משימה זו.  להלן דוגמה לשינוי מדיניות הפגישה הגלובלית עבור הארגון שלך.   

(הקפד לסקור את התיעוד לעיל לפני ביצוע שינויים אלה כדי להבין בדיוק מה זה מאפשר.)

סט מדיניות-הAllowPSTNUsersToBypassLobby הכללית של זהות המשתמש "כולם"-מ$True

לקבלת מידע נוסף, ראה [הגדרת מדיניות מוגדרת](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).
