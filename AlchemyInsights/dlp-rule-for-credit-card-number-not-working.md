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
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005091"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>בעיות DLP במספרי כרטיסי אשראי

**חשוב**: בתקופה חסרת תקדים זאת, אנחנו נוקטים בצעדים כדי להבטיח ששירותי SharePoint Online ו- OneDrive יישארו בזמינות גבוהה - לקבלת מידע נוסף, בקר בכתובת [התאמות של תכונה זמנית ב- SharePoint Online](https://aka.ms/ODSPAdjustments).

**בעיות DLP במספרי כרטיסי אשראי**

האם אתה נתקל בבעיות **במניעת אובדן נתונים (DLP)** לא פועל עבור תוכן המכיל מספר כרטיס אשראי בעת שימוש בסוג מידע רגיש של DLP ב- O365?  אם כן, ודא שהתוכן שלך מכיל את המידע הדרוש כדי להפעיל את מדיניות DLP כאשר הוא מוערך. לדוגמה, עבור מדיניות **כרטיס אשראי** המוגדרת עם רמת ביטחון של 85%, הפריטים הבאים מוערכים ויש לזהות אותם כדי שהכלל יפעיל:
  
- **[עיצוב:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 ספרות ההן יכולות להיות מעוצבות או לא מעוצבות (dddddddddddddd) ועליה להעביר את מחשב.

- **[תבנית:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** דפוס מורכב ורב-צורה המאתר כרטיסים מכל המותגים העיקריים ברחבי העולם, כולל ויזה, MasterCard, Discover Card, JCB, American Express, כרטיסי מתנה וכרטיסי דיינר.

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** כן, בדיקת ה- Checksum של Luhn

- **[הגדרה:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** מדיניות DLP בטוחה ב- 85% שהיא זיהתה סוג זה של מידע רגיש אם, בקרבה של 300 תווים:

  - הפונקציה Func_credit_card תוכן שמתאים לתבנית.

  - אחת מהאפשרויות הבאות היא true:

  - מילת מפתח Keyword_cc_verification נמצאת.

  - מילת מפתח Keyword_cc_name נמצאת

  - הפונקציה Func_expiration_date תאריך בתבנית התאריך הנכונה.

  - בדיקת ההמחאה עוברת

    לדוגמה, הדוגמה הבאה תפעיל מדיניות מספר כרטיס אשראי של DLP:

  - ויזה: 4485 3647 3952 7352
  
  - פג: 2/02/09

לקבלת מידע נוסף על מה  שנדרש כדי לזהות מספר כרטיס אשראי עבור התוכן שלך, עיין בסעיף הבא במאמר זה: מה סוגי המידע [הרגישים מחפשים כרטיס אשראי#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
באמצעות סוג מידע רגיש מוכלל אחר, עיין במאמר הבא לקבלת מידע אודות מה נדרש עבור סוגים אחרים: [מה סוגי המידע הרגישים מחפשים](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  