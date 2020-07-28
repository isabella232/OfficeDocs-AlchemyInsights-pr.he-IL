---
title: איתור התקנים אבודים iOS עם Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439626"
---
# <a name="locating-lost-ios-devices-with-intune"></a>איתור התקנים אבודים iOS עם Intune

הפעלת מצב אבוד בהתקן iOS מאפשרת למנהל לנהל הודעה ומספר טלפון של איש קשר המוצגים על מסך הנעילה.

לאחר שמצב ' אבד ' מופעל, המנהל יכול להשתמש בפעולת ההתקן אתר כדי לזהות את המיקום הפיזי של ההתקן.

פעולת ההתקן אתר ב-Intune עובדת עם התקני iOS כדי להציג את המיקום של התקן מסוים על המפה.

שימוש בפעולה זו מחייב את התקן iOS להיות ב:

- מצב פיקוח
- מצב אבוד

לקבלת מידע נוסף, ראה [הפעלת מצב אבוד על ios/ipados התקנים עם Intune](https://docs.microsoft.com/intune/device-lost-mode) [ולאתר אובדן או נגנב Ios/ipados התקנים עם Intune](https://docs.microsoft.com/intune/device-locate).

**שאלות נפוצות**

ש: הנפקת פעולה מרוחקת כדי להסיר נתוני חברה מהתקן, וכעת היא תקועה במצב המתנה.

ת: כדי שפעולה מרוחקת תושלם בהצלחה, ההתקן המיועד חייב להיות מקוון ובריא. במצבים הבאים, הפעולה המרוחקת נשארת במצב המתנה למשך 30 יום, או עד שההתקן מכיר את הפקודה:

- כאשר אין להתקן קישוריות
- כאשר ההתקן מאבד את מצב הניהול שלו עם Intune

אם אתה סבור שהתקן אינו נמצא עוד בבדיקה ושהוא לא יוכל להסיר נתוני חברה, בחר במחק. מחיקה מסירה את רשומת ההתקן כך שלא תופיע עוד ברשימת ההתקנים Intune. אם ההתקן הופך לפעיל שוב, המשתמש יצטרך לרשום אותו מחדש.

ש: מדוע פעולות מרוחקות מסוימות אינן זמינות עבורי לשימוש?

ת: לא כל הפלטפורמות תומכות בכל פעולות ההתקן המרוחק. הפעולות המרוחקות הבאות הן ספציפיות לפלטפורמה, ולכן הן זמינות רק עבור הפלטפורמות שצוינו.

- עקיפת נעילת הפעלה (iOS בלבד)
- התחלה חדשה (Windows בלבד)
- מצב אבוד (iOS בלבד)
- אתר התקן (iOS בלבד)
- הפעל מחדש (Windows בלבד)

לקבלת פרטים נוספים אודות כל פעולה, ראה [פעולות התקן זמינות](https://docs.microsoft.com/intune/device-management#available-device-actions).