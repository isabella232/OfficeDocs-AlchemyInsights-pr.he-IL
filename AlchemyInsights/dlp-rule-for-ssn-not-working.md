---
title: כלל DLP for SSN אינו פועל
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679370"
---
# <a name="dlp-issues-with-social-security-numbers"></a>בעיות של DLP עם מספרי תעודת זהות

**חשוב**: בתקופה חסרת תקדים זאת, אנחנו נוקטים בצעדים כדי להבטיח ששירותי SharePoint Online ו- OneDrive יישארו בזמינות גבוהה - לקבלת מידע נוסף, בקר בכתובת[התאמות של תכונה זמנית ב- SharePoint Online](https://aka.ms/ODSPAdjustments).

**בעיות ב-DLP עם SSNs**

האם אתה נתקל בבעיות **במניעת אובדן נתונים (DLP)** לא פועל עבור תוכן המכיל **מספר תעודת זהות (SSN)** בעת שימוש בסוג מידע רגיש ב-Microsoft 365? אם כן, ודא שהתוכן שלך מכיל את המידע הדרוש עבור מראה מדיניות ה-DLP. 
  
לדוגמה, עבור מדיניות SSN שתצורתה נקבעה עם רמת בטחון של 85%, הערכים הבאים מוערכים ויש לזהות אותם עבור הכלל לגורם מפעיל:
  
- **[עיצוב:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 ספרות, שעשויות להופיע בתבנית מעוצבת או לא מעוצבת

- **[תבנית:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** ארבע פונקציות מחפשות SSNs בארבע תבניות שונות:

  - Func_ssn מוצא את SSNs עם עיצוב חזק של pre-2011 המעוצב עם מקפים או רווחים (ddd-dd-dddd או ddd dd dddd)

  - Func_unformatted_ssn מוצא את SSNs עם עיצוב חזק של pre-2011 שאינו מעוצב כתשעה ספרות רצופות (ddddddddd)

  - Func_randomized_formatted_ssn מוצא את post-2011 SSNs המעוצב עם מקפים או רווחים (ddd-dd-dddd או ddd dd dddd)

  - Func_randomized_unformatted_ssn מוצא את post-2011 SSNs שאינם מעוצבים כתשעה ספרות רצופות (ddddddddd)

- **[בדיקת סיכום:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** לא, אין בדיקת סיכום

- **[הגדרה:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** מדיניות DLP היא 85% בטוח שהיא זיהתה סוג זה של מידע רגיש אם בתוך סמיכות של 300 תווים:

  - [הפונקציה Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) מאתרת תוכן התואם לתבנית.

  - מילת מפתח מתוך [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) מתקיימת. דוגמאות למילות מפתח כוללות: ביטוח  *לאומי, ביטוח לאומי, Soc שניה, SSN*  . לדוגמה, המדגם הבא יגרום להפעלת מדיניות SSN של DLP: **SSN: 489-36-8350**
  
לקבלת מידע נוסף אודות הנדרש עבור SSNs לצורך זיהוי עבור התוכן שלך, עיין בסעיף הבא במאמר זה: [מה סוגי המידע הרגישים מחפשים את SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
באמצעות סוג מידע מוכלל אחר שונה, עיין במאמר הבא לקבלת מידע על הדרישות הדרושות עבור סוגים אחרים: [מה סוגי המידע הרגישים מחפשים](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  