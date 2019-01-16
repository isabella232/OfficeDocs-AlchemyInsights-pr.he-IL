---
title: טכנולוגיית DLP כלל עבור מספר הביטוח הלאומי אינו פועל
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b92d122b774d97cd2e44cc0880dc5001065b57cc
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28291885"
---
האם אתה נתקל בבעיות עם **מניעת אובדן נתונים (DLP)** אינה פועלת עבור תוכן המכיל של **מספר הביטוח הלאומי (SSN)** בעת שימוש בסוג מידע רגיש ב- Office 365? אם כן, ודא כי התוכן שלך מכיל את המידע הדרוש עבור המידע הדרוש מדיניות DLP. 
  
לדוגמה, עבור מדיניות SSN נקבעה עם רמת הביטחון של 85%, הבאות מוערכים ואת אפשרות לזהות עבור הכלל להפעיל:
  
- **[תבנית:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 ספרות, שעשוי להיות בתבנית מעוצב או לא מעוצב 
    
- **[תבנית:](https://msconnect.microsoft.com/https:/docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** ארבע פונקציות חפש את SSNs ארבע תבניות שונות: 
    
  - Func_ssn מוצא SSNs עם טרום-2011 עיצוב חזק המעוצבים באמצעות מקפים או רווחים (או ddd-dd-dddd ddd dddd dd)
    
  - Func_unformatted_ssn מוצא SSNs עם טרום-2011 עיצוב חזק שהם לא מעוצב תשע ספרות עוקבים (ddddddddd)
    
  - Func_randomized_formatted_ssn מוצא SSNs post-2011 המעוצבים באמצעות מקפים או רווחים (או ddd-dd-dddd ddd dddd dd)
    
  - Func_randomized_unformatted_ssn מוצא SSNs post-2011 שהם לא מעוצב תשע ספרות עוקבים (ddddddddd)
    
- **[בדיקת סיכום:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** לא, קיימת ללא בדיקת סיכום 
    
- **[הגדרה:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** מדיניות DLP הוא 85% בטוח כי סוג זה של מידע רגיש זיהה if, בתוך מידת הקירבה של 300 תווים: 
    
  - [הפונקציה Func_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) מחפש תוכן התואם את התבנית. 
    
  - נמצאה מילת מפתח מתוך [Keyword_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) . כולל דוגמאות של מילות מפתח: *לאומי, לאומי #, Soc שניה, מספר תעודת זהות* . לדוגמה, להפעיל דוגמת הבאה עבור המדיניות DLP SSN: **מספר תעודת זהות: 489-36-8350**
    
לקבלת מידע נוסף אודות מה נדרש עבור SSNs לאתר עבור התוכן שלך, עיין בסעיף הבא במאמר זה: [מה ה רגיש סוגי מידע מחפשים SSNs](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
באמצעות סוג אחר מידע רגיש מוכללים, ראה את המאמר הבא לקבלת מידע על מה נדרש עבור סוגים אחרים: [מה ה רגיש סוגי מידע לחפש](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

