---
title: כלל DLP של מספר כרטיס אשראי שאינו פועל
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 80ff41b3e746f95278ccbf0df19eebb61f7f9ee0
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704202"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP בעיות עם מספרי כרטיסי אשראי

**חשוב**: בתקופה חסרת תקדים זאת, אנחנו נוקטים בצעדים כדי להבטיח ששירותי SharePoint Online ו- OneDrive יישארו בזמינות גבוהה - לקבלת מידע נוסף, בקר בכתובת[התאמות של תכונה זמנית ב- SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP בעיות עם מספרי כרטיסי אשראי**

האם אתה נתקל בבעיות **במניעת אובדן נתונים (DLP)** שאינן פועלות עבור תוכן המכיל **מספר כרטיס אשראי** בעת שימוש בסוג מידע רגיש של DLP ב-O365? אם כן, ודא שהתוכן שלך מכיל את המידע הדרוש כדי להפעיל את מדיניות ה-DLP כאשר הוא מוערך. לדוגמה, עבור **מדיניות כרטיס אשראי** שהוגדרה באמצעות רמת ביטחון של 85%, ההערכה הבאה מוערכת ויש לאתרם כדי שהכלל יפעיל:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 ספרות שניתן לעצב או לא מעוצב (dddddddddd) וחייב לעבור את מבחן luhn.

- **[תבנית:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** תבנית מורכבת ואיתנה מאוד המזהה קלפים מכל המותגים הגדולים בעולם, כולל ויזה, מאסטרקארד, דיסקקארד, JCB, אמריקן אקספרס, כרטיסי מתנה וכרטיסי סועד.

- **[בדיקת סיכום:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** כן, בדיקת הסיכום של Luhn

- **[הגדרה:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** מדיניות DLP היא 85% בטוחה שהיא זיהתה סוג זה של מידע רגיש אם, בסמיכות של 300 תווים:

  - הפונקציה Func_credit_card מאתרת תוכן התואם לתבנית.

  - אחד מהבאים מתקיים:

  - נמצאה מילת מפתח מKeyword_cc_verification.

  - נמצאה מילת מפתח מKeyword_cc_name

  - הפונקציה Func_expiration_date מאתרת תאריך בתבנית התאריך המתאימה.

  - בדיקת הסיכום עוברת

    לדוגמה, הדוגמה הבאה תפעיל מדיניות מספר כרטיס אשראי של DLP:

  - ויזה: 4485 3647 3952 7352
  
  - תאריך תפוגה: 2/2009

לקבלת מידע נוסף אודות הדרוש עבור **מספר כרטיס אשראי** שיזוהה עבור התוכן שלך, עיין בסעיף הבא במאמר זה: [מה סוגי המידע הרגישים מחפשים כרטיס אשראי](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
באמצעות סוג מידע רגיש ומובנה שונה, עיין במאמר הבא לקבלת מידע אודות הדרוש עבור סוגים אחרים: [מה סוגי המידע הרגישים מחפשים](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  