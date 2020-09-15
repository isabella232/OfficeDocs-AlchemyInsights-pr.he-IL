---
title: כלל DLP עבור מספר כרטיס אשראי אינו פועל
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679442"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>בעיות של DLP עם מספרי כרטיסי אשראי

**חשוב**: בתקופה חסרת תקדים זאת, אנחנו נוקטים בצעדים כדי להבטיח ששירותי SharePoint Online ו- OneDrive יישארו בזמינות גבוהה - לקבלת מידע נוסף, בקר בכתובת[התאמות של תכונה זמנית ב- SharePoint Online](https://aka.ms/ODSPAdjustments).

**בעיות של DLP עם מספרי כרטיסי אשראי**

האם אתה נתקל בבעיות **במניעת אובדן נתונים (DLP)** לא עובד עבור תוכן המכיל **מספר כרטיס אשראי** בעת שימוש בסוג מידע רגיש של DLP ב-O365? אם כן, ודא שהתוכן שלך מכיל את המידע הדרוש כדי להפעיל את מדיניות ה-DLP כאשר היא מוערכת. לדוגמה, עבור **מדיניות כרטיס אשראי** שתצורתה נקבעה באמצעות רמת בטחון של 85%, הערכים הבאים מוערכים ויש לזהות אותם עבור הכלל לגורם מפעיל:
  
- **[עיצוב:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 ספרות שניתן לעצב או לא לעצב (dddddddddddddddd) ולהעביר את הבדיקה Luhn.

- **[תבנית:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** תבנית מורכבת וחזקה מאוד המזהה קלפים מכל המותגים העיקריים ברחבי העולם, כולל ויזה, מסטרקארד, כרטיס מגלה, JCB, אמריקן אקספרס, כרטיסי מתנה וכרטיסי סועד.

- **[בדיקת סיכום:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** כן, בדיקת הסיכום של Luhn

- **[הגדרה:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** מדיניות DLP היא 85% בטוח שהיא זיהתה סוג זה של מידע רגיש אם בתוך סמיכות של 300 תווים:

  - הפונקציה Func_credit_card מאתרת תוכן התואם לתבנית.

  - אחת מהאפשרויות הבאות היא true:

  - מילת מפתח מתוך Keyword_cc_verification מתקיימת.

  - מילת מפתח מתוך Keyword_cc_name מאותרת

  - הפונקציה Func_expiration_date מאתרת תאריך בתבנית התאריך המתאימה.

  - בדיקת הסיכום מעבירה

    לדוגמה, המדגם הבא יגרום להפעלת מדיניות מספר כרטיס אשראי של DLP:

  - ויזה: 4485 3647 3952 7352
  
  - תוקף התוקף: 2/2009

לקבלת מידע נוסף אודות הנדרש עבור **מספר כרטיס אשראי** שיזוהה עבור התוכן שלך, עיין בסעיף הבא במאמר זה: [מה סוגי המידע הרגישים מחפשים כרטיס אשראי](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
באמצעות סוג מידע מוכלל אחר שונה, עיין במאמר הבא לקבלת מידע על הדרישות הדרושות עבור סוגים אחרים: [מה סוגי המידע הרגישים מחפשים](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  