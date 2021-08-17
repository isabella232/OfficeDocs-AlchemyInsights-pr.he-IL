---
title: חיפוש אירועים המבוצעים בכללי תיבת דואר נכנס
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
ms.openlocfilehash: d6a4eadd897dfae3b65ccda6363edfe9cef1c810
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313500"
---
# <a name="find-events-performed-on-inbox-rules"></a>חיפוש אירועים המבוצעים בכללי תיבת דואר נכנס

כאשר כללי תיבת דואר נכנס נוצרים, משתנים או נמחקים, האירועים מתועדים ביומן הביקורת. כך ת לסקור אותם:

1. ביצוע אחת מהפעולות הבאות:
   - בתיבת מרכז התאימות של Microsoft 365 <https://compliance.microsoft.com> at , עבור אל **ביקורת** \> **פתרונות**. לחלופין, כדי לעבור ישירות **לדף ביקורת,** השתמש <https://compliance.microsoft.com/auditlogsearch> ב- .
   - בפורטל Microsoft 365 Defender <https://security.microsoft.com> ב- , עבור אל **ביקורת**. לחלופין, כדי לעבור ישירות **לדף ביקורת,** השתמש <https://security.microsoft.com/auditlogsearch> ב- .

    **הערה:** אם אתה רואה הודעה שתצטרך להפעיל ביקורת, הפעל אותה כעת. אם תכונה זו אינה מופעלת, תוצאות החיפוש לא יוכלו למשוך נתונים מתאריכים קודמים.
1. בחר את השדה פעילויות ומצא Exchange תיבת דואר ולאחר מכן בחר New-InboxRule צור כלל תיבת דואר נכנס מתוך Outlook Web App. לאחר סיימת, לחץ מחוץ לחלונית כדי למזער את החלונית פעילויות.
1. ציין את טווח התאריכים ולאחר מכן, בשדה משתמשים, בחר את שם המשתמש עבור המשתמש שברצונך לחקור. באפשרותך לבחור יותר ממשתמש אחד בכל פעם.
1. בחר חיפוש. הפעילויות מופיעות תחת תוצאות.
1. כדי להציג פרטים, בחר פעילות ולאחר מכן בחר מידע נוסף. תחת המקטע פרמטרים, באפשרותך לראות את שם הכלל, ערכת התנאים והפעולות שהכלל יקבע.

2. בכרטיסיה חיפוש **בדף** ביקורת, **הגדר** את ההגדרות הבאות:
   - **טווח תאריך ושעה:** בחר את טווח התאריך/שעה **בתיבות** **התחלה** וסיום.
   - **פעילויות**: בחר **כלל תיבת דואר נכנס חדשה-InboxRule Create from Outlook Web App**

3. כשתסיים, לחץ על **חיפוש**. הפעילויות מופיעות בדף **החיפוש החדש 'ביקורת'.**

4. בחר פעילות בתוצאות כדי לפתוח את הפרטים נשלף. תחת **המקטע פרמטרים,** באפשרותך לראות את שם הכלל, ערכת התנאים והפעולות שהכלל יקבע.

כדי ללמוד עוד, ראה [חיפוש ביומן הביקורת כדי לבדוק בעיות תמיכה נפוצות](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
