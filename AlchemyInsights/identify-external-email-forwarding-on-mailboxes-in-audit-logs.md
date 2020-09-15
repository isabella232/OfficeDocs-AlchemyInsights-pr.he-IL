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
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696298"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>זיהוי כאשר העברת דואר אלקטרוני חיצונית מוגדרת בתיבות דואר

כאשר משתמש של Microsoft 365 קובע את התצורה של העברת דואר אלקטרוני חיצוני בתיבת דואר, הפעילות מתבצעת ביקורת כחלק מ **-Cmdlet Set-mailbox** . באפשרותך לראות את הפעילות באמצעות חיפוש ביומן הביקורת במרכז התאימות של אבטחה &.

1. היכנס [למרכז התאימות של Microsoft 365 Security &](https://protection.office.com/).

2. עבור אל דף **Search**  >  **החיפוש ביומן ביקורת** חיפוש.

3. בחר את טווח התאריכים בשדות **תאריך התחלה** **ותאריך סיום** . אין צורך לציין שם משתמש. אימות השדה ' **פעילויות** ' מוגדר **לתצוגת תוצאות עבור כל הפעילויות**.

4. לחץ על **חיפוש**.

בתוצאות, לחץ על **סנן תוצאות** והקלד **ערכת תיבת דואר** בתיבה מסנן פעילות. בחר רשומת ביקורת בתוצאות. בנשלף של **הפרטים** , לחץ על **מידע נוסף**. עליך לעיין בפרטים של כל רשומת ביקורת כדי לקבוע אם הפעילות קשורה להעברת דואר אלקטרוני.

- **ObjectId**: ערך הכינוי של תיבת הדואר שהשתנתה.

- **פרמטרים**: _ForwardingSmtpAddress_ מציין את כתובת הדואר האלקטרוני המהווה יעד.

- **מזהה**משתמש: המשתמש שהגדיר את העברת הדואר האלקטרוני בתיבת הדואר בשדה **ObjectId** .

לקבלת מידע נוסף, ראה [קביעה מי הגדיר העברת דואר אלקטרוני עבור תיבת דואר](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
