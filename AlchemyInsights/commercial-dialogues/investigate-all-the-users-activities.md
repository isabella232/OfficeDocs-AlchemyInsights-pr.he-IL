---
title: לחקור את כל הפעילויות של המשתמשים
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: d05c8f02efc3bb92865880ea4a2338abaf7d70254f0b4bbfb566423e62b391dd
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898797"
---
# <a name="investigate-all-the-users-activities"></a>לחקור את כל הפעילויות של המשתמשים

כך ניתן לעשות זאת:

1. ביצוע אחת מהפעולות הבאות:
   - בתיבת מרכז התאימות של Microsoft 365 <https://compliance.microsoft.com> at , עבור אל **ביקורת** \> **פתרונות**. לחלופין, כדי לעבור ישירות **לדף ביקורת,** השתמש <https://compliance.microsoft.com/auditlogsearch> ב- .
   - בפורטל Microsoft 365 Defender <https://security.microsoft.com> ב- , עבור אל **ביקורת**. לחלופין, כדי לעבור ישירות **לדף ביקורת,** השתמש <https://security.microsoft.com/auditlogsearch> ב- .

    > [!NOTE]
    > אם אתה רואה הודעה שתצטרך להפעיל את התכונה, הפעל אותה כעת. אם התכונה לא מופעלת, תוצאות החיפוש לא יוכלו למשוך נתונים מתאריכים קודמים.

2. בכרטיסיה חיפוש **בדף** ביקורת, **הגדר** את ההגדרות הבאות:
   - **טווח תאריך ושעה:** בחר את טווח התאריך/שעה **בתיבות** **התחלה** וסיום.
   - **פעילויות**: אם אתה מעוניין בפעילות ספציפית, בחר אותה מהרשימה; אחרת, ערך ברירת המחדל **הצג תוצאות עבור כל הפעילויות מחזיר** את כל הפעילויות.
   - **משתמשים**: קבל את ערך ברירת המחדל הריק כדי להחזיר תוצאות עבור כל המשתמשים, או הזן משתמש אחד או יותר.

3. כשתסיים, לחץ על **חיפוש**. הפעילויות מופיעות בדף **החיפוש החדש 'ביקורת'.** תראה את כתובת **ה- IP**, **המשתמש** ואת **שם** הפעילות.

4. כדי להוריד את התוצאות, בחר **ייצוא הורד** את \> **כל התוצאות**.

5. בחר פעילות בתוצאות כדי לפתוח את הפרטים נשלף.

כדי ללמוד עוד, ראה [חיפוש ביומן הביקורת כדי לבדוק בעיות תמיכה נפוצות](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
