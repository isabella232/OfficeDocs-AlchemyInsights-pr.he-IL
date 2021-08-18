---
title: זיהוי העברת דואר אלקטרוני חיצונית בתיבות דואר ביומני ביקורת
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 2af731bc9a1e28e2db7c6662041b930e1b05be4c3bf8340784d9ab87101c44af
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57899885"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>זהה מתי העברת דואר אלקטרוני חיצונית מוגדרת בתיבות דואר

כאשר משתמש Microsoft 365 מגדיר העברת דואר אלקטרוני חיצונית בתיבת דואר, הפעילות מבוקרת כחלק מ- **cmdlet Set-Mailbox.** באפשרותך לראות את הפעילות באמצעות חיפוש יומן ביקורת. כך ניתן לעשות זאת.

1. בצע אחד מהשלבים הבאים:
   - בתיבת מרכז התאימות של Microsoft 365 <https://compliance.microsoft.com> at , עבור אל **ביקורת** \> **פתרונות**. לחלופין, כדי לעבור ישירות **לדף ביקורת,** השתמש <https://compliance.microsoft.com/auditlogsearch> ב- .
   - בפורטל Microsoft 365 Defender <https://security.microsoft.com> ב- , עבור אל **ביקורת**. לחלופין, כדי לעבור ישירות **לדף ביקורת,** השתמש <https://sip.security.microsoft.com/auditlogsearch> ב- .

2. בדף **ביקורת,** ודא שהכרטיסייה חיפוש **נבחרה** ולאחר מכן קבע את תצורת ההגדרות הבאות:
   - בחר את טווח התאריך/שעה **בתיבות** התחלה **וסיום.**
   - ודא **שהתיבה** פעילויות **מכילה הצג תוצאות עבור כל הפעילויות.**

3. כשתסיים, לחץ על **חיפוש**. הפעילויות מופיעות בדף **החיפוש החדש 'ביקורת'.**

4. בתוצאות, לחץ על **סינון תוצאות** והקלד **Set-Mailbox** בתיבת מסנן הפעילות.

5. בחר רשומת ביקורת בתוצאות. ב- **פרטים** נשלף, לחץ **על מידע נוסף**. עליך לתעד את הפרטים של כל רשומת ביקורת כדי לקבוע אם הפעילות קשורה להעברת דואר אלקטרוני.

   - **ObjectId**: ערך הכינוי של תיבת הדואר ששונתה.
   - **פרמטרים**: _ForwardingSmtpAddress מציין_ את כתובת הדואר האלקטרוני של היעד.
   - **UserId**: המשתמש שקבע את תצורת העברת הדואר האלקטרוני בתיבת הדואר **בשדה ObjectId.**

לקבלת מידע נוסף, [ראה קביעת מי הגדיר העברת דואר אלקטרוני עבור תיבת דואר](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
