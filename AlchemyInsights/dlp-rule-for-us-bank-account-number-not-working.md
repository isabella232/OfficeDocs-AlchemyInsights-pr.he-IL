---
title: כלל DLP עבור מספר חשבון בנק של US אינו פועל
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
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005019"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>בעיות DLP במספרי חשבון בנק של US

**חשוב**: בתקופה חסרת תקדים זאת, אנחנו נוקטים בצעדים כדי להבטיח ששירותי SharePoint Online ו- OneDrive יישארו בזמינות גבוהה - לקבלת מידע נוסף, בקר בכתובת [התאמות של תכונה זמנית ב- SharePoint Online](https://aka.ms/ODSPAdjustments).

**בעיות DLP במספרי חשבון בנק של US**

האם אתה נתקל בבעיות **במניעת אובדן נתונים (DLP)** לא פועל עבור תוכן המכיל מספר חשבון בנק של **US** בעת שימוש בסוג מידע רגיש של DLP ב- O365? אם כן, ודא שהתוכן שלך מכיל את המידע הדרוש עבור המדיניות של DLP מחפשת כאשר הוא מוערך.
  
לדוגמה, עבור **מדיניות מספר חשבון** בנק של US שתצורתה נקבעה עם רמת ביטחון של 85%, הפעולות הבאות מוערכות ויש לזהותן כדי שהכלל יפעיל:
  
- **[עיצוב:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 ספרות

- **[תבנית:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 ספרות רצופות.

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** לא, אין 'בדיקת המחאה'

- **[הגדרה:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** מדיניות DLP בטוחה ב- 75% שהיא זיהתה סוג זה של מידע רגיש אם, בקרבה של 300 תווים:

  - הביטוי הרגיל Regex_usa_bank_account_number תוכן שמתאים לתבנית

  - מילת מפתח Keyword_usa_Bank_Account נמצאת.

    לדוגמה, הדוגמה הבאה תפעיל את **מדיניות מספר חשבון** הבנק של US: בדיקת חשבון 78344011

לקבלת מידע נוסף על מה  שנדרש כדי לזהות את מספר חשבון הבנק של US עבור התוכן שלך, עיין בסעיף הבא במאמר זה: מה סוגי המידע [הרגישים מחפשים את מספר חשבון הבנק של US](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
באמצעות סוג מידע רגיש מוכלל אחר, עיין במאמר הבא לקבלת מידע אודות מה נדרש עבור סוגים אחרים: [מה סוגי המידע הרגישים מחפשים](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  