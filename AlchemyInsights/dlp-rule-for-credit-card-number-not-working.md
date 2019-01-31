---
title: טכנולוגיית DLP כלל עבור מספר כרטיס האשראי אינו פועל
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 4b8897c5cc8286bc4bd49860658a5a94ad17380d
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657468"
---
האם אתה נתקל בבעיות עם **מניעת אובדן נתונים (DLP)** אינה פועלת עבור תוכן המכיל **מספר כרטיס האשראי** בעת שימוש בסוג מידע רגיש DLP ב- O365? אם כן, ודא כי התוכן שלך מכיל את המידע הדרוש כדי להפעיל המדיניות DLP כאשר חישובו. לדוגמה, עבור **כרטיס אשראי מדיניות** מוגדרת עם רמת הביטחון של 85%, הבאות מוערכים ואת אפשרות לזהות עבור הכלל להפעיל: 
  
- **[תבנית:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 ספרות אשר ניתן לעצב או לא מעוצב (dddddddddddddddd) ואת חייבת לעבור מחשב Luhn. 
    
- **[תבנית:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** תבנית מורכבים מאוד ולא יציב שמזהה קלפים מתוך כל המותגים העיקריים ברחבי העולם, כולל ויזה, Mastercard, לגלות כרטיס, JCB, אמריקן אקספרס, כרטיסי מתנה, וכרטיסי דיינרס. 
    
- **[בדיקת סיכום:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** כן, בדיקת הסיכום Luhn 
    
- **[הגדרה:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** מדיניות DLP הוא 85% בטוח כי סוג זה של מידע רגיש זיהה if, בתוך מידת הקירבה של 300 תווים: 
    
  - הפונקציה Func_credit_card מחפש תוכן התואם את התבנית.
    
  - אחד מהצעדים הבאים מתקיים: 
    
  - נמצאה מילת מפתח מתוך Keyword_cc_verification.
    
  - נמצאה מילת מפתח מתוך Keyword_cc_name
    
  - הפונקציה Func_expiration_date מוצא תאריך בתבנית התאריך הנכון.
    
  - מעביר בדיקת סיכום
    
    לדוגמה, דוגמת הבאה יחזיר עבור מדיניות מספר כרטיס אשראי מסוג DLP:
    
  - ויזה: 4485 3647 3952 7352 
    
  - פג תוקף: 2/2009
    
לקבלת מידע נוסף אודות מה נדרש עבור **מספר כרטיס האשראי** לאתר עבור התוכן שלך, עיין בסעיף הבא במאמר זה: [מה ה רגיש סוגי מידע לחפש כרטיס אשראי #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
באמצעות סוג אחר מידע רגיש מוכללים, ראה את המאמר הבא לקבלת מידע על מה נדרש עבור סוגים אחרים: [מה ה רגיש סוגי מידע לחפש](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

