---
title: כלל DLP עבור ארה ב / אנגליה מספר דרכון לא עובד
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: ec7f11676982b56a46c83bf276c2212ce765ba6f
ms.sourcegitcommit: ca06ef831226d629de3057a0df85e017b80f3356
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/08/2019
ms.locfileid: "29786699"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>בעיות עם טכנולוגיית DLP - ארה ב / אנגליה Passport מספרים

האם אתה נתקל בבעיות עם **מניעת אובדן נתונים (DLP)** לא עובד המכיל תוכן **ארה ב / מספר דרכון בבריטניה** בעת שימוש בסוג מידע רגיש DLP ב- O365? אם כן, ודא כי התוכן שלך מכיל את המידע הדרוש עבור מה המדיניות DLP הוא מחפש כאשר חישובו. 
  
לדוגמה, עבור **ארה ב / מספר דרכון בבריטניה** מוגדרת עם רמת הביטחון של 75%, הבאות מוערכים והמדיניות אפשרות לזהות עבור כלל להנעת 
  
- **[תבנית:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** תשע ספרות 
    
- **[תבנית:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** תשע ספרות עוקבים 
    
- **[בדיקת סיכום:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** לא, קיימת ללא בדיקת סיכום 
    
- **[הגדרה:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** מדיניות DLP הוא 75% בטוח כי סוג זה של מידע רגיש זיהה if, בתוך מידת הקירבה של 300 תווים: 
    
  - הפונקציה Func_usa_uk_passport מחפש תוכן התואם את התבנית.
    
  - נמצאה מילת מפתח מתוך Keyword_passport.
    
    לדוגמה, להפעיל דוגמת הבאה עבור **ארה ב / מספר דרכון בבריטניה** מדיניות: מספר דרכון אמריקאי 123456789 
    
לקבלת מידע נוסף אודות מה נדרש עבור ארה ב / אנגליה מספר דרכון לאתר עבור התוכן שלך, עיין בסעיף הבא במאמר זה: [מראה מה ה רגיש סוגי מידע עבור ארצות הברית / מספר דרכון בבריטניה](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
באמצעות סוג אחר מידע רגיש מוכללים, ראה את המאמר הבא לקבלת מידע על מה נדרש עבור סוגים אחרים: [מה ה רגיש סוגי מידע לחפש](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

