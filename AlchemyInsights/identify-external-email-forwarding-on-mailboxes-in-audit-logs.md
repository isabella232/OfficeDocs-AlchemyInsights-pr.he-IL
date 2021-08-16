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
ms.openlocfilehash: 1e80917a323128ba23175651cdf4d892d7815a89c1223b654812c1b456c787da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028739"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>זהה מתי העברת דואר אלקטרוני חיצונית מוגדרת בתיבות דואר

כאשר משתמש Microsoft 365 מגדיר העברת דואר אלקטרוני חיצונית בתיבת דואר, הפעילות מבוקרת כחלק מ- **cmdlet Set-Mailbox.** באפשרותך לראות את הפעילות באמצעות חיפוש יומן ביקורת במרכז האבטחה & תאימות.

1. היכנס למרכז [Microsoft 365 התאימות.](https://protection.office.com/)

2. עבור אל דף **החיפוש של**  >  **יומן ביקורת** החיפוש.

3. בחר את טווח התאריכים בשדות **תאריך התחלה** **ותאריך** סיום. אין צורך לציין שם משתמש. ודא **שהשדות פעילויות** מוגדרים **להצגת תוצאות עבור כל הפעילויות.**

4. לחץ **על חיפוש**.

בתוצאות, לחץ על **סינון תוצאות** והקלד **Set-Mailbox** בתיבת מסנן הפעילות. בחר רשומת ביקורת בתוצאות. ב- **פרטים** נשלף, לחץ **על מידע נוסף**. עליך לבדוק את הפרטים של כל רשומת ביקורת כדי לקבוע אם הפעילות קשורה להעברת דואר אלקטרוני.

- **ObjectId**: ערך הכינוי של תיבת הדואר ששונתה.

- **פרמטרים**: _ForwardingSmtpAddress מציין_ את כתובת הדואר האלקטרוני של היעד.

- **UserId**: המשתמש שקבע את תצורת העברת הדואר האלקטרוני בתיבת הדואר **בשדה ObjectId.**

לקבלת מידע נוסף, [ראה קביעת מי הגדיר העברת דואר אלקטרוני עבור תיבת דואר](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
