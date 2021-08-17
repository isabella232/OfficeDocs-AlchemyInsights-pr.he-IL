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
ms.openlocfilehash: 7746e44a0ee5a4442051900985aab339b09652f08e412b02a02429c93cc7c107
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57895180"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>גלה מי הגדיר העברה בתיבת דואר ואופן ההעברה

אם העברה חיצונית הוגדר בתיבת דואר, הפעילות מבוקרת כחלק מ- **cmdlet Set-Mailbox.** כך תמצא את הפעילות ביומן הביקורת:

1. ביצוע אחת מהפעולות הבאות:
   - בתיבת מרכז התאימות של Microsoft 365 <https://compliance.microsoft.com> at , עבור אל **ביקורת** \> **פתרונות**. לחלופין, כדי לעבור ישירות **לדף ביקורת,** השתמש <https://compliance.microsoft.com/auditlogsearch> ב- .
   - בפורטל Microsoft 365 Defender <https://security.microsoft.com> ב- , עבור אל **ביקורת**. לחלופין, כדי לעבור ישירות **לדף ביקורת,** השתמש <https://security.microsoft.com/auditlogsearch> ב- .

   > [!NOTE]
   > אם אתה רואה הודעה שאתה צריך להפעיל ביקורת, הפעל אותה כעת. אם תכונה זו אינה מופעלת, תוצאות החיפוש לא יוכלו למשוך נתונים מתאריכים קודמים.

2. בדף **ביקורת,** ודא שהכרטיסייה חיפוש **נבחרה** ולאחר מכן קבע את תצורת ההגדרות הבאות:
   - בחר את טווח התאריך/שעה **בתיבות** התחלה **וסיום.**
   - ודא **שהתיבה** פעילויות **מכילה הצג תוצאות עבור כל הפעילויות.**

3. כשתסיים, לחץ על **חיפוש**. הפעילויות מופיעות בדף **החיפוש החדש 'ביקורת'.**

4. בתוצאות, לחץ על תיבת **עמודה** כדי למיין את התוצאות ולחפש **ערכי Set-Mailbox.**

5. בחר פעילות בתוצאות כדי לפתוח את הפרטים נשלף. עליך לבדוק את הפרטים של כל רשומת ביקורת כדי לקבוע אם הפעילות קשורה להעברת דואר אלקטרוני:
   - **ObjectId**: ערך הכינוי של תיבת הדואר ששונתה.
   - **פרמטרים**: _ForwardingSmtpAddress מציין_ את כתובת הדואר האלקטרוני של היעד.
   - **UserId**: המשתמש שקבע את תצורת העברת הדואר האלקטרוני בתיבת הדואר **בשדה ObjectId.**

לקבלת מידע נוסף, [ראה קביעת מי הגדיר העברת דואר אלקטרוני עבור תיבת דואר](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
