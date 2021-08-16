---
title: כלל DLP עבור מספר הדרכון של ארה"ב/בריטניה אינו פועל
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004947"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>בעיות ב- DLP - מספרי דרכון של ארה"ב/בריטניה

**חשוב**: בתקופה חסרת תקדים זאת, אנחנו נוקטים בצעדים כדי להבטיח ששירותי SharePoint Online ו- OneDrive יישארו בזמינות גבוהה - לקבלת מידע נוסף, בקר בכתובת [התאמות של תכונה זמנית ב- SharePoint Online](https://aka.ms/ODSPAdjustments).

**בעיות DLP במספרי דרכון של ארה"ב/בריטניה**

האם אתה נתקל בבעיות **במניעת אובדן נתונים (DLP)** לא פועל עבור תוכן המכיל מספר דרכון של **ארה"ב/בריטניה** בעת שימוש בסוג מידע רגיש של DLP ב- O365? אם כן, ודא שהתוכן שלך מכיל את המידע הדרוש עבור המדיניות של DLP מחפשת כאשר הוא מוערך.
  
לדוגמה, עבור מדיניות מספר דרכון של **ארה"ב/בריטניה** שתצורתה נקבעה עם רמת ביטחון של 75%, הפעולות הבאות מוערכות ויש לזהותן כדי שהכלל יפעיל
  
- **[עיצוב:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** תשע ספרות

- **[תבנית:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** תשע ספרות רצופות

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** לא, אין 'בדיקת המחאה'

- **[הגדרה:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** מדיניות DLP בטוחה ב- 75% שהיא זיהתה סוג זה של מידע רגיש אם, בקרבה של 300 תווים:

  - הפונקציה Func_usa_uk_passport את התוכן שמתאים לתבנית.

  - מילת מפתח Keyword_passport נמצאת.

    לדוגמה, הדוגמה הבאה תפעיל את מדיניות מספר הדרכון **בארה"ב/בריטניה:** מספר דרכון 123456789

לקבלת מידע נוסף על מה שנדרש כדי לזהות את מספר ה- Passport של ארה"ב/בריטניה עבור התוכן שלך, עיין בסעיף הבא במאמר זה: כיצד סוגי המידע הרגישים מחפשים את [מספר הדרכון של ארה"ב/בריטניה](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
באמצעות סוג מידע רגיש מוכלל אחר, עיין במאמר הבא לקבלת מידע אודות מה נדרש עבור סוגים אחרים: [מה סוגי המידע הרגישים מחפשים](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  