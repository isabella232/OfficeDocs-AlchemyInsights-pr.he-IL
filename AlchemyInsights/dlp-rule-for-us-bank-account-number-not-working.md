---
title: טכנולוגיית DLP כלל עבור לנו מספר חשבון הבנק אינו פועל
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0a32708b5ac8d95ec6777ada2d151a15f90d65bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529869"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>בעיות מסוג DLP עם מספרי חשבון בנק לנו

האם אתה נתקל בבעיות עם **מניעת אובדן נתונים (DLP)** אינה פועלת עבור תוכן המכיל **מספר חשבון בנק בארה ב** בעת שימוש בסוג מידע רגיש DLP ב- O365? אם כן, ודא כי התוכן שלך מכיל את המידע הדרוש עבור מה המדיניות DLP הוא מחפש כאשר חישובו.
  
לדוגמה, עבור מדיניות **מספר חשבון בנק בארה ב** נקבעה עם רמת הביטחון של 85%, הבאות מוערכים ואת אפשרות לזהות עבור הכלל להפעיל:
  
- **[עיצוב:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 ספרות

- **[תבנית:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 ספרות עוקבים.

- **[בדיקת סיכום:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** לא, קיימת ללא בדיקת סיכום

- **[הגדרה:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** מדיניות DLP הוא 75% בטוח כי סוג זה של מידע רגיש זיהה if, בתוך מידת הקירבה של 300 תווים:

  - הביטוי הרגיל Regex_usa_bank_account_number מוצא תוכן התואם את התבנית

  - נמצאה מילת מפתח מתוך Keyword_usa_Bank_Account.

    לדוגמה, להפעיל דוגמת הבאה עבור מדיניות **מספר חשבון בנק בארה ב** : 78344011 חשבון עו ש

לקבלת מידע נוסף אודות מה נדרש עבור **מספר חשבון בנק בארה ב** לזהות עבור התוכן שלך, עיין בסעיף הבא במאמר זה: [מה ה רגיש סוגי מידע מחפשים מספר חשבון בנק בארה ב](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
באמצעות סוג אחר מידע רגיש מוכללים, ראה את המאמר הבא לקבלת מידע על מה נדרש עבור סוגים אחרים: [מה ה רגיש סוגי מידע לחפש](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  