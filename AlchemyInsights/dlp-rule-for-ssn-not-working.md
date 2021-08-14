---
title: כלל DLP עבור SSN אינו פועל
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
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004983"
---
# <a name="dlp-issues-with-social-security-numbers"></a>בעיות DLP במספרי ביטוח לאומי

**חשוב**: בתקופה חסרת תקדים זאת, אנחנו נוקטים בצעדים כדי להבטיח ששירותי SharePoint Online ו- OneDrive יישארו בזמינות גבוהה - לקבלת מידע נוסף, בקר בכתובת [התאמות של תכונה זמנית ב- SharePoint Online](https://aka.ms/ODSPAdjustments).

**בעיות DLP עם SSN**

האם אתה נתקל בבעיות **במניעת אובדן נתונים (DLP)** לא פועל עבור תוכן המכיל מספר תעודת **זהות (SSN)** בעת שימוש בסוג מידע רגיש ב- Microsoft 365? אם כן, ודא שהתוכן שלך מכיל את המידע הדרוש עבור מה שמדיניות DLP מחפשת. 
  
לדוגמה, עבור מדיניות SSN שתצורתה נקבעה עם רמת ביטחון של 85%, הפריטים הבאים מוערכים ויש לזהות אותם כדי שהכלל יפעיל:
  
- **[עיצוב:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 ספרות, העשויות להיות בתבנית מעוצבת או לא מעוצבת

- **[תבנית:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** ארבע פונקציות מחפשות SSNs בארבע תבניות שונות:

  - Func_ssn את SSNs עם עיצוב חזק מראש 2011 המעוצב עם מקפים או רווחים (ddd-dd-dddd OR ddd dd dddd)

  - Func_unformatted_ssn את SSNs עם עיצוב חזק של קדם-2011 שלא מעוצבים כ- 9 ספרות רצופות (ddddddddd)

  - Func_randomized_formatted_ssn איתור SSN post-2011 המעוצבים באמצעות מקפים או רווחים (ddd-dd-dddd OR dddd ddd dd dddd dddd)

  - Func_randomized_unformatted_ssn איתור SSN שלאחר 2011 שלא מעוצבים כ- 9 ספרות רצופות (ddddddddd)

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** לא, אין 'בדיקת המחאה'

- **[הגדרה:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** מדיניות DLP בטוחה ב- 85% שהיא זיהתה סוג זה של מידע רגיש אם, בקרבה של 300 תווים:

  - הפונקציה [Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) תוכן שמתאים לתבנית.

  - מילת מפתח [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) נמצאת. דוגמאות למילות מפתח כוללות:  *Social Security, Social Security#, Soc Sec ,SSN*  . לדוגמה, הדוגמה הבאה תפעיל עבור מדיניות SSN של **DLP: SSN: 489-36-8350**
  
לקבלת מידע נוסף על מה שנדרש לזיהוי SSN עבור התוכן שלך, עיין בסעיף הבא במאמר זה: מה סוגי המידע [הרגישים מחפשים SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
באמצעות סוג מידע רגיש מוכלל אחר, עיין במאמר הבא לקבלת מידע אודות מה נדרש עבור סוגים אחרים: [מה סוגי המידע הרגישים מחפשים](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  