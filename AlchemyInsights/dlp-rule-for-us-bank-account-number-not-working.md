---
title: כלל DLP של מספר חשבון בנק בארה ב אינו פועל
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: b032a7c80e8b387114aeda95c4f6af7e57225517
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507335"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP בעיות עם מספרי חשבונות בנק בארה ב

**חשוב**: בתקופה חסרת תקדים זאת, אנחנו נוקטים בצעדים כדי להבטיח ששירותי SharePoint Online ו- OneDrive יישארו בזמינות גבוהה - לקבלת מידע נוסף, בקר בכתובת[התאמות של תכונה זמנית ב- SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP בעיות עם מספרי חשבונות בנק בארה ב**

האם אתה נתקל בבעיות עם **מניעת אובדן נתונים (DLP)** שאינם פועלים עבור תוכן המכיל **מספר חשבון בנק בארה** ב בעת שימוש בסוג מידע רגיש של DLP ב-O365? אם כן, ודא שהתוכן שלך מכיל את המידע הדרוש עבור מה שמדיניות DLP מחפשת בעת חישובו.
  
לדוגמה, עבור מדיניות **מספר חשבון בנק של ארה"ב** המוגדרת ברמת ביטחון של 85%, ההערכה הבאה מוערכת ויש לאתרם כדי שהכלל יפעיל:
  
- [**תבנית:**](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77) 8-17 ספרות

- [**תבנית:**](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77) 8-17 ספרות רצופות.

- [**בדיקת סיכום:**](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76) לא, אין בדיקת סיכום

- [**הגדרה:**](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions) מדיניות DLP היא 75% בטוחה שהיא זיהתה סוג זה של מידע רגיש אם, בסמיכות של 300 תווים:

  - הביטוי הרגיל Regex_usa_bank_account_number מוצא תוכן התואם לתבנית

  - נמצאה מילת מפתח מ-Keyword_usa_Bank_Account.

    לדוגמה, הדוגמה הבאה תפעיל את מדיניות **מספר חשבון הבנק של ארה"ב** : בדיקת חשבון 78344011

לקבלת מידע נוסף אודות הדרוש עבור **מספר חשבון בנק של ארה"ב** שיזוהה עבור התוכן שלך, עיין בסעיף הבא במאמר זה: [מה סוגי המידע הרגישים מחפשים מספר חשבון בנק US](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
באמצעות סוג מידע רגיש ומובנה שונה, עיין במאמר הבא לקבלת מידע אודות הדרוש עבור סוגים אחרים: [מה סוגי המידע הרגישים מחפשים](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  