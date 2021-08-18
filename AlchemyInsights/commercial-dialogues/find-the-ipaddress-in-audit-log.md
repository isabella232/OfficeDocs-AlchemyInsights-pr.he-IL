---
title: חיפוש כתובת ה- IP ביומן הביקורת
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: c3b1cac5379f4f3da93152fa20086068f7df562cd98b2980ce1b4280e0aa6d5f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57902261"
---
# <a name="find-the-ip-address-in-audit-log"></a>חיפוש כתובת ה- IP ביומן הביקורת

כתובת ה- IP התואמת לפעילות שבוצעה על-ידי משתמש או מנהל מערכת מוצגת ביומני הביקורת. פרטי הלקוח נרשם גם הם. כך תוכל לזהות את כתובת ה- IP:

1. ביצוע אחת מהפעולות הבאות:
   - בתיבת מרכז התאימות של Microsoft 365 <https://compliance.microsoft.com> at , עבור אל **ביקורת** \> **פתרונות**. לחלופין, כדי לעבור ישירות **לדף ביקורת,** השתמש <https://compliance.microsoft.com/auditlogsearch> ב- .
   - בפורטל Microsoft 365 Defender <https://security.microsoft.com> ב- , עבור אל **ביקורת**. לחלופין, כדי לעבור ישירות **לדף ביקורת,** השתמש <https://security.microsoft.com/auditlogsearch> ב- .

    > [!NOTE]
    > אם אתה רואה הודעה שאתה צריך להפעיל ביקורת, הפעל אותה כעת. אם תכונה זו אינה זמינה, תוצאות החיפוש לא יוכלו למשוך נתונים מתאריכים קודמים.

2. בדף **ביקורת,** ודא שהכרטיסייה חיפוש **נבחרה** ולאחר מכן קבע את תצורת ההגדרות הבאות:
   - **טווח תאריך ושעה:** בחר את טווח התאריך/שעה **בתיבות** **התחלה** וסיום.
   - **פעילויות**: אם אתה מעוניין בפעילות ספציפית, בחר אותה מהרשימה; אחרת, ערך ברירת **המחדל הצג תוצאות עבור כל הפעילויות** מחזיר את כל הפעילויות יוחזרו.. שים לב שייתכן שפעילויות מסוימות לא יהיו זמינות לבחירה; עם זאת, פריטי ביקורת אלה יוחזרו **אם האפשרות הצג תוצאות עבור כל** הפעילויות נבחרה.
   - **משתמשים**: קבל את ערך ברירת המחדל הריק כדי להחזיר תוצאות עבור כל המשתמשים, או הזן משתמש אחד או יותר.

3. כשתסיים, לחץ על **חיפוש**. הפעילויות מופיעות בדף **החיפוש החדש 'ביקורת'.**

4. בתוצאות, לחץ על **סינון תוצאות** והקלד **Set-Mailbox** בתיבת מסנן הפעילות.

5. בחר רשומת ביקורת בתוצאות כדי לפתוח את הפריט **נשלף** פרטים.

לקבלת מידע נוסף, ראה [חיפוש ביומן הביקורת כדי לבדוק בעיות תמיכה נפוצות](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
