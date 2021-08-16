---
title: גלה מי הגדיר העברה בתיבת דואר ואופן ההעברה
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
ms.openlocfilehash: 6243e787bb6b51f26cf22782d9ec80f946430b864f53de7ea626b7166a674d2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988202"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>גלה מי הגדיר העברה בתיבת דואר ואופן ההעברה

אם העברה חיצונית הוגדר בתיבת דואר, הפעילות מבוקרת כחלק מ- cmdlet Set-Mailbox ה- cmdlet. כך תמצא את הפעילות ביומן הביקורת:

1. עבור אל [Office 365 האבטחה & תאימות](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. בחר **חיפוש בחיפוש** ביומן >  **ביקורת**.
    > [!NOTE]
    > אם אתה רואה הודעה שאתה צריך להפעיל ביקורת, הפעל אותה כעת. אם תכונה זו אינה מופעלת, תוצאות החיפוש לא יוכלו למשוך נתונים מתאריכים קודמים.
1. ודא כי השדה **פעילויות** מוגדר להציג תוצאות **עבור כל הפעילויות (ברירת** המחדל). ציין את טווח התאריכים. אין צורך לציין שם משתמש.
1. בחר **חפש**. הפעילויות מופיעות תחת **תוצאות**.
1. בחר **סינון תוצאות** ולאחר מכן הזן **Set-mailbox** בשדה **מסנן** פעילות. פעולה זו מחזירה את **כל פעילויות Set-Mailbox.**
1. כדי להציג את הפרטים, בחר פעילות ולאחר מכן בחר **מידע נוסף**. תחת **פרמטרים,** באפשרותך לראות את כתובת הדואר האלקטרוני להעברה הוגדר בתיבת הדואר. מזהה **המשתמש מייצג** את המשתמש שהגדיר העברה חיצונית בתיבת הדואר.
כדי ללמוד עוד, ראה [חיפוש ביומן Office 365 ביקורת כדי לפתור בעיות בתרחישים נפוצים](https://go.microsoft.com/fwlink/?linkid=2103944).