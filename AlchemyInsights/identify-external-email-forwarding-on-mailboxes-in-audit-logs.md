---
title: זיהוי העברת דואר אלקטרוני חיצוני בתיבות דואר ביומני ביקורת
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716461"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>זיהוי כאשר תצורת העברת דואר אלקטרוני חיצונית מוגדרת בתיבות דואר

כאשר משתמש של Microsoft 365 מגדיר העברה של דואר אלקטרוני חיצוני בתיבת דואר, הפעילות מתבצעת ביקורת כחלק מיישומון ה **-Cmdlet Set-mailbox** . באפשרותך לראות את הפעילות באמצעות חיפוש יומן ביקורת במרכז התאימות של אבטחה _ אמפר _.

1. היכנס ל- [Microsoft 365 האבטחה _ אמפר _ מרכז התאימות](https://protection.office.com/).

2. עבור אל דף **Search** > **החיפוש של יומן ביקורת** חיפוש.

3. בחר את טווח התאריכים **בתאריך ההתחלה** ושדות **הסיום** . אין צורך לציין שם משתמש. ודא שהשדה **פעילויות** מוגדר **להצגת תוצאות עבור כל הפעילויות**.

4. לחץ על **חיפוש**.

בתוצאות, לחץ על **סנן תוצאות** וסוג **ערכת תיבות דואר** בתיבה מסנן פעילות. בחר רשומת ביקורת בתוצאות. בתפריט **הפרטי** , לחץ על **מידע נוסף**. עליך לבדוק את הפרטים של כל רשומת ביקורת כדי לקבוע אם הפעילות קשורה להעברת דואר אלקטרוני.

- **אובייtid**: ערך הכינוי של תיבת הדואר שהשתנתה.

- **פרמטרים**: _כתובת השולח_ מציינת את כתובת האימייל של היעד.

- **Userid**: המשתמש שהגדיר העברת דואר אלקטרוני בתיבת הדואר בשדה **אובייtid** .

לקבלת מידע נוסף, ראה [קביעה מי הגדיר העברת דואר אלקטרוני עבור תיבת דואר](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
