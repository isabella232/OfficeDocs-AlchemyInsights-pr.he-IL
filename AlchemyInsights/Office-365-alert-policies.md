---
title: 1385-Office-365-alert-policies
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 681f7609f32b004ddfa7bfbeff179757e7063657
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312688"
---
# <a name="alert-policies"></a>מדיניות התראה

Microsoft 365 [מכיל](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) פריטי מדיניות התראה המהווים ברירת מחדל שמפעילים התראות עבור ארגונים עם מנוי Microsoft 365 Enterprise או Microsoft 365 US Government E1/G1, E3/G3 או E5/G5. לכן, מנהלי מערכת עשויים לקבל הודעת דואר אלקטרוני של התראה Office365Alerts@microsoft.com באמצעות שורת נושא כגון "התראת חומרה נמוכה: *שם מדיניות התראה*". הודעות התראה נשלחות כאשר התראות מופעלות עבור פעילויות נפוצות, כגון כאשר משתמשים:

- צור כללי תיבת דואר נכנס ההעברות דואר אלקטרוני.
- הקצה הרשאות לתיבת הדואר שלהם.
- שתף או מחק מספר גדול של קבצים SharePoint קבצים.
- צור חיפושים של גילוי אלקטרוני וייצוא של תוצאות חיפוש.

כדי לסקור התראה ולפעל אותה:

1. בצע אחד מהשלבים הבאים:
   - בתיבת מרכז התאימות של Microsoft 365 , <https://compliance.microsoft.com> עבור אל **התראות**. לחלופין, כדי לעבור ישירות **לדף 'התראות',** השתמש <https://compliance.microsoft.com/compliancealerts> ב- .
   - בפורטל Microsoft 365 Defender <https://security.microsoft.com> , עבור אל **אירועים &** \> **התראות**. לחלופין, כדי לעבור ישירות **לדף 'התראות',** השתמש <https://security.microsoft.com/alerts> ב- .
2. לחץ על התראה כדי להציג דף נשלף עם מידע אודות ההתראה.

באפשרותך לבצע פעולה בהתראה, כגון הסרת [כלל חשוד של תיבת דואר נכנס](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account). לחלופין, באפשרותך פשוט לסגור את ההתראה על-ידי לחיצה **על פתור** בדף נשלף ההתראה.

לקבלת מידע נוסף אודות קביעת תצורה וניהול של מדיניות התראה, עיין  [במאמר זה](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).

**חשוב**: התראה על הודעות דואר אלקטרוני מ- Microsoft לעולם לא יבקשו ממך לעשות את הפעולות הבאות:

- ספק סיסמה
- אימות פרטי האבטחה של החשבון שלך
- אימות מחדש של עצמך

אם אתה מקבל הודעת דואר אלקטרוני עם סוגים אלה של בקשות, היא לא נשלחה על-ידי Microsoft ויש להיחשב להונאת דיוג. אם אתה מקבל הודעה עם סוגים אלה של בקשות, [הדוח את ההודעה ל- Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft).
