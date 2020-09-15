---
title: כלל DLP עבור מספר הדרכון של ארה ב/בריטניה אינו פועל
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
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679225"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>בעיות במספרי הדרכון של DLP-US/UK

**חשוב**: בתקופה חסרת תקדים זאת, אנחנו נוקטים בצעדים כדי להבטיח ששירותי SharePoint Online ו- OneDrive יישארו בזמינות גבוהה - לקבלת מידע נוסף, בקר בכתובת[התאמות של תכונה זמנית ב- SharePoint Online](https://aka.ms/ODSPAdjustments).

**בעיות ב-DLP עם מספרי הדרכון של ארה ב/בריטניה**

האם אתה נתקל בבעיות **במניעת אובדן נתונים (DLP)** לא עובד עבור תוכן המכיל **מספר דרכון אמריקאי/בריטי** בעת שימוש בסוג מידע רגיש של DLP ב-O365? אם כן, ודא שהתוכן שלך מכיל את המידע הדרוש עבור הפעולות שבהן מדיניות DLP מחפשת כאשר היא מוערכת.
  
לדוגמה, עבור מדיניות **מספרי הדרכון של ארה"ב/UK** שהוגדרה ברמת ביטחון של 75%, הערכים הבאים מוערכים ויש לזהות אותם עבור הכלל למפעיל
  
- **[תבנית:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** תשע ספרות

- **[תבנית:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** תשע ספרות רצופות

- **[בדיקת סיכום:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** לא, אין בדיקת סיכום

- **[הגדרה:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** מדיניות DLP היא 75% בטוח שהיא זיהתה סוג זה של מידע רגיש אם בתוך סמיכות של 300 תווים:

  - הפונקציה Func_usa_uk_passport מאתרת תוכן התואם לתבנית.

  - מילת מפתח מתוך Keyword_passport מתקיימת.

    לדוגמה, המדגם הבא יפעיל את מדיניות **מספרי הדרכון של ארה"ב/UK** : מספר 123456789 של U.S. passport

לקבלת מידע נוסף אודות הנדרש עבור מספר דרכון אמריקאי/בריטי שיזוהה עבור התוכן שלך, עיין בסעיף הבא במאמר זה: [מה סוגי המידע הרגישים מחפשים מספר דרכון של ארה"ב/uk](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
באמצעות סוג מידע מוכלל אחר שונה, עיין במאמר הבא לקבלת מידע על הדרישות הדרושות עבור סוגים אחרים: [מה סוגי המידע הרגישים מחפשים](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  