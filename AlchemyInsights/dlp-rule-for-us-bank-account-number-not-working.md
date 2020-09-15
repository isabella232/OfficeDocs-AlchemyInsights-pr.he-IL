---
title: מספר חשבון הבנק של DLP for US אינו פועל
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679297"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>בעיות ב-DLP עם מספרי חשבון בנק ארה"ב

**חשוב**: בתקופה חסרת תקדים זאת, אנחנו נוקטים בצעדים כדי להבטיח ששירותי SharePoint Online ו- OneDrive יישארו בזמינות גבוהה - לקבלת מידע נוסף, בקר בכתובת[התאמות של תכונה זמנית ב- SharePoint Online](https://aka.ms/ODSPAdjustments).

**בעיות ב-DLP עם מספרי חשבון בנק ארה"ב**

האם אתה נתקל בבעיות **במניעת אובדן נתונים (DLP)** לא פועל עבור תוכן המכיל **מספר חשבון בנק אמריקאי** בעת שימוש בסוג מידע רגיש של DLP ב-O365? אם כן, ודא שהתוכן שלך מכיל את המידע הדרוש עבור הפעולות שבהן מדיניות DLP מחפשת כאשר היא מוערכת.
  
לדוגמה, עבור מדיניות **מספר חשבון בנק של ארה"ב** המוגדרת עם רמת ביטחון של 85%, הערכים הבאים מוערכים ויש לזהות אותם עבור הכלל לגורם מפעיל:
  
- **[עיצוב:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 ספרות

- **[תבנית:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 ספרות רצופות.

- **[בדיקת סיכום:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** לא, אין בדיקת סיכום

- **[הגדרה:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** מדיניות DLP היא 75% בטוח שהיא זיהתה סוג זה של מידע רגיש אם בתוך סמיכות של 300 תווים:

  - הביטוי הרגיל Regex_usa_bank_account_number מוצא תוכן שמתאים לתבנית

  - מילת מפתח מתוך Keyword_usa_Bank_Account מתקיימת.

    לדוגמה, הדוגמה הבאה תגרום להפעלת מדיניות **מספר חשבון בנק ארה"ב** : בדיקת חשבון 78344011

לקבלת מידע נוסף אודות הנדרש עבור **מספר חשבון בנק אמריקאי** שיאותר עבור התוכן שלך, עיין בסעיף הבא במאמר זה: [מה סוגי המידע הרגישים מחפשים מספר חשבון בנק בארה](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
באמצעות סוג מידע מוכלל אחר שונה, עיין במאמר הבא לקבלת מידע על הדרישות הדרושות עבור סוגים אחרים: [מה סוגי המידע הרגישים מחפשים](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  