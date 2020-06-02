---
title: כלל DLP של מספר דרכון בארה ב/בבריטניה אינו פועל
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 3d3b7dc2d9510376bc9eef6ec69b87ad7c681b05
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507299"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>בעיות עם מספרי הדרכון של DLP-US/בריטניה

**חשוב**: בתקופה חסרת תקדים זאת, אנחנו נוקטים בצעדים כדי להבטיח ששירותי SharePoint Online ו- OneDrive יישארו בזמינות גבוהה - לקבלת מידע נוסף, בקר בכתובת[התאמות של תכונה זמנית ב- SharePoint Online](https://aka.ms/ODSPAdjustments).

**בעיות DLP של מספרי דרכון בארה ב/בבריטניה**

האם אתה נתקל בבעיות עם **מניעת אובדן נתונים (DLP)** שאינה פועלת עבור תוכן המכיל **מספר דרכון בארה ב/בבריטניה** בעת שימוש בסוג מידע רגיש של DLP ב-O365? אם כן, ודא שהתוכן שלך מכיל את המידע הדרוש עבור מה שמדיניות DLP מחפשת בעת חישובו.
  
לדוגמה, עבור מדיניות **מספר דרכון של ארה"ב/UK** המוגדרת עם רמת ביטחון של 75%, ההערכה הבאה מוערכת ויש לאתרם כדי שהכלל יפעיל
  
- [**תבנית:**](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77) תשע ספרות

- [**תבנית:**](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77) תשע ספרות רצופות

- [**בדיקת סיכום:**](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76) לא, אין בדיקת סיכום

- [**הגדרה:**](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77) מדיניות DLP היא 75% בטוחה שהיא זיהתה סוג זה של מידע רגיש אם, בסמיכות של 300 תווים:

  - הפונקציה Func_usa_uk_passport מאתרת תוכן התואם לתבנית.

  - נמצאה מילת מפתח מKeyword_passport.

    לדוגמה, הדוגמה הבאה תפעיל את מדיניות **מספר הדרכון ארה ב/בריטניה** : דרכון מספר 123456789 בארה ב

לקבלת מידע נוסף אודות הנדרש עבור מספר Passport של ארה ב/בריטניה שיזוהה עבור התוכן שלך, עיין בסעיף הבא במאמר זה: [מה סוגי המידע הרגישים מחפשים מספר דרכון בארה ב/בריטניה](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
באמצעות סוג מידע רגיש ומובנה שונה, עיין במאמר הבא לקבלת מידע אודות הדרוש עבור סוגים אחרים: [מה סוגי המידע הרגישים מחפשים](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  