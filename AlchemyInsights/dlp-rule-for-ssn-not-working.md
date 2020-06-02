---
title: כלל DLP עבור SSN אינו פועל
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 35859bce89ef1ae9b6a9e706fc316b0ee6cd27d1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507371"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP בעיות עם מספרי ביטוח לאומי

**חשוב**: בתקופה חסרת תקדים זאת, אנחנו נוקטים בצעדים כדי להבטיח ששירותי SharePoint Online ו- OneDrive יישארו בזמינות גבוהה - לקבלת מידע נוסף, בקר בכתובת[התאמות של תכונה זמנית ב- SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP בעיות עם SSNs**

האם אתה נתקל בבעיות עם **מניעת אובדן נתונים (DLP)** אינה פועלת עבור תוכן המכיל **מספר תעודת זהות (SSN)** בעת שימוש בסוג מידע רגיש ב-Microsoft 365? אם כן, ודא שהתוכן שלך מכיל את המידע הדרוש עבור מה שמדיניות ה-DLP מחפשת. 
  
לדוגמה, עבור מדיניות SSN המוגדרת עם רמת ביטחון של 85%, ההערכה הבאה מוערכת ויש לאתרם כדי שהכלל יפעיל:
  
- [**תבנית:**](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80) 9 ספרות, שעשויות להיות בתבנית מעוצבת או לא מאותחלת

- [**תבנית:**](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) ארבע פונקציות מחפש SSNs בארבעה דפוסים שונים:

  - Func_ssn מוצא SSNs עם עיצוב חזק של pre-2011 המעוצבים באמצעות מקפים או רווחים (ddd-dd-dddd או ddd dd dddd)

  - Func_unformatted_ssn מוצא SSNs עם עיצוב חזק של pre-2011 שאינם מתוכנתים כתשע ספרות רצופות (ddddddddd)

  - Func_randomized_formatted_ssn מאתרת SSNs שלאחר 2011 המעוצבים באמצעות מקפים או רווחים (ddd-dd-dddd או ddd dd dddd)

  - Func_randomized_unformatted_ssn מוצאת SSNs שלאחר 2011 שאינם מאותחלת כתשע ספרות רצופות (ddddddddd)

- [**בדיקת סיכום:**](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79) לא, אין בדיקת סיכום

- [**הגדרה:**](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80) מדיניות DLP היא 85% בטוחה שהיא זיהתה סוג זה של מידע רגיש אם, בסמיכות של 300 תווים:

  - [הפונקציה Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) מאתרת תוכן התואם לתבנית.

  - נמצאה מילת מפתח מ- [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) . דוגמאות של מילות מפתח כולל: *ביטוח לאומי, ביטוח לאומי, Soc שניה, SSN* . לדוגמה, הדוגמה הבאה תפעיל את מדיניות DLP SSN: **SSN: 489-36-8350**
  
לקבלת מידע נוסף אודות הדרוש עבור SSNs שיזוהו עבור התוכן שלך, עיין בסעיף הבא במאמר זה: [מה סוגי המידע הרגישים מחפשים SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
באמצעות סוג מידע רגיש ומובנה שונה, עיין במאמר הבא לקבלת מידע אודות הדרוש עבור סוגים אחרים: [מה סוגי המידע הרגישים מחפשים](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  