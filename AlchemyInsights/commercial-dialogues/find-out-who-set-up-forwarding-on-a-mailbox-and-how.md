---
title: גלה מי הגדיר העברה בתיבת דואר וכיצד
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482297"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>גלה מי הגדיר העברה בתיבת דואר וכיצד

אם הוגדרה העברה חיצונית בתיבת דואר, הפעילות מתבצעת ביקורת כחלק מ-cmdlet הSet-Mailbox. כך תוכל למצוא את הפעילות ביומן הביקורת:

1. עבור אל [מרכז התאימות & אבטחה של Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. בחר חיפוש >  **ביומן הביקורת** של חיפוש.
    > [!NOTE]
    > אם אתה רואה הודעה שעליך להפעיל את הביקורת, הפעל אותה כעת. אם תכונה זו אינה מופעלת, תוצאות החיפוש לא יוכלו למשוך נתונים מתאריכים קודמים.
1. ודא שהשדה **פעילויות** מוגדר **להציג תוצאות עבור כל הפעילויות** (ברירת המחדל). ציין את טווח התאריכים. אין צורך לציין שם משתמש.
1. בחר **חיפוש**. הפעילויות מופיעות תחת **תוצאות**.
1. בחר באפשרות **מסנן תוצאות** ולאחר מכן הזן **Set-mailbox** בשדה מסנן **פעילות** . פעולה זו מחזירה את כל פעילויות **הערכה-תיבת דואר** .
1. כדי להציג את הפרטים, בחר פעילות ולאחר מכן בחר **מידע נוסף**. תחת **פרמטרים** באפשרותך לראות את כתובת הדואר האלקטרוני להעברה שהוגדרה בתיבת הדואר. **מזהה** המשתמש מייצג את המשתמש שהגדיר העברה חיצונית בתיבת הדואר.
לקבלת מידע נוסף, ראה [חיפוש ביומן הביקורת של Office 365 כדי לפתור תרחישים נפוצים](https://go.microsoft.com/fwlink/?linkid=2103944).