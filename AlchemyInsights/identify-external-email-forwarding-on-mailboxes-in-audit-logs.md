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
ms.openlocfilehash: b7146b2b09b6ac1e33b192dcbcbfb72ea2593313
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630250"
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
