---
title: לזהות העברת דואר אלקטרוני חיצוני על תיבות דואר ביומני ביקורת
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 518e4dd485ee7c54ce83e65794152e32f4c3a836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752002"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>לזהות בעת העברת דואר אלקטרוני חיצוני נקבעה עבור תיבות דואר

כאשר משתמש מגדיר את העברת דואר אלקטרוני חיצוני דואר, הפעילות תתבצע ביקורת כחלק cmdlet **Set-Mailbox** . באפשרותך לראות את הפעילות באמצעות חיפוש יומן ביקורת ב- & אבטחה מרכז תאימות.

1. היכנס אל [מרכז התאימות של Office 365 אבטחה &](https://protection.office.com/)

2. לחץ על **חיפוש ויצירת החקירה** ובחר באפשרות **החיפוש יומן ביקורת**.

3. בחר את טווח התאריכים בשדות **תאריך התחלה** ותאריך **סיום** . אין צורך לציין שם משתמש. ודא שהשדה **פעילויות** מוגדר להצגת **תוצאות עבור כל הפעילויות**.

4. לחץ על **חיפוש**.

בתוצאות, לחץ על **סינון תוצאות** והקלד **Set-Mailbox** בתיבה מסנן פעילות. בחר את רשומת הביקורת בתוצאות. תפריט נשלף של **פרטים** , לחץ על **מידע נוסף**. יש לך להסתכל על הפרטים של כל רשומת הביקורת כדי לקבוע אם הפעילות קשורה דוא ל העברה.

- **ObjectId**: הערך הכינוי של תיבת הדואר שהשתנה.

- **פרמטרים**: _ForwardingSmtpAddress_ מציין את כתובת הדואר האלקטרוני של היעד.

- **מזהה משתמש**: המשתמש שתצורתו נקבעה העברת דואר אלקטרוני בתיבת הדואר בשדה **ObjectId** .

לקבלת מידע נוסף, ראה [קביעת שהגדיר העברה עבור תיבת דואר אלקטרוני](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
