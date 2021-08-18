---
title: קריאת יומני הביקורת עבור אירועים שנמחקו
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
ms.openlocfilehash: ec8f845f599e397814bc9077c3fe59edb5324192
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324734"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>קריאת יומני הביקורת עבור אירועים שנמחקו

כך ניתן לעשות זאת:

1. ביצוע אחת מהפעולות הבאות:
   - בתיבת מרכז התאימות של Microsoft 365 , <https://compliance.microsoft.com> עבור אל **ביקורת** \> **פתרונות**. לחלופין, כדי לעבור ישירות **לדף ביקורת,** השתמש <https://compliance.microsoft.com/auditlogsearch> ב- .
   - בפורטל Microsoft 365 Defender <https://security.microsoft.com> ב- , עבור אל **ביקורת**. לחלופין, כדי לעבור ישירות **לדף ביקורת,** השתמש <https://security.microsoft.com/auditlogsearch> ב- .

    **הערה:** אם אתה רואה הודעה שתצטרך להפעיל את התכונה, הפעל אותה כעת. אם התכונה לא מופעלת, תוצאות החיפוש לא יוכלו למשוך נתונים מתאריכים קודמים.

2. בכרטיסיה חיפוש **בדף** ביקורת, **הגדר** את ההגדרות הבאות:
   - **טווח תאריך ושעה:** בחר את טווח התאריך/שעה **בתיבות** **התחלה** וסיום.
   - **פעילויות**: **הזן Exchange תיבת הדואר** ולאחר מכן בחר את הערכים הבאים:
     - **הודעות שנמחקו מהתיקיה 'פריטים שנמחקו'**
     - **העברת הודעות לתיקיה 'פריטים שנמחקו'**

       לאחר סיימת, לחץ מחוץ לחלונית כדי למזער את **החלונית** פעילויות.

   - **משתמשים**: קבל את ערך ברירת המחדל הריק כדי להחזיר תוצאות עבור כל המשתמשים, או הזן משתמש אחד או יותר.

3. כשתסיים, לחץ על **חיפוש**. הפעילויות מופיעות בדף **החיפוש החדש 'ביקורת'.**

4. בחר פעילות בתוצאות כדי לפתוח את הפרטים נשלף. מידע נוסף אודות הפריט שנמחק, כגון שורת הנושא ומיקום הפריט בעת מחיקתו, מוצג בשדה **AffectedItems.**

   **הערה:** לא ניתן לשחזר פריטים שנמחקו באמצעות תכונת יומן הביקורת. כדי לשחזר פריטים שנמחקו, ראה [שחזור הודעות דואר אלקטרוני שנמחקו ב- Outlook באינטרנט](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11).

לקבלת מידע נוסף, ראה [חיפוש ביומן הביקורת כדי לבדוק בעיות תמיכה נפוצות](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
