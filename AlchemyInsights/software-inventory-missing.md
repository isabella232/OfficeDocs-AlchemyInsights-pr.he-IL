---
title: מלאי התוכנה חסר או לא מדויק
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676266"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a>מלאי התוכנה חסר או לא מדויק

מלאי התוכנה ב- Threat and Vulnerability Management (TVM) הוא רשימה של תוכנות ידועות בארגון שלך עם ספירות פלטפורמה נפוצות רשמיות (CPE).

מוצרי תוכנה ללא CPE רשמי לא פורסמו פגיעויות. המלאי כולל גם פרטים כגון שם הספק, מספר החולשות, האיומים ומספר המכשירים החשופים.

שינויי תוכנה במכשירים משתקפים בדרך כלל בפורטלים של אבטחה תוך שעתיים. עם זאת, ייתכן שלפעמים זה יקח זמן רב יותר. בשלב זה אין דרך לכפות סינכרון; זוהי הערכה רציפה מתמשכת.

אם ביצעת שינוי תוכנה והשינוי אינו משתקף ב- TVM לאחר 5 שעות, בצע את הפעולות הבאות:

1. בדוק את מקטע הראיות של התוכנה כדי להבין כיצד זוהתה התוכנה.
1. ודא שהתוכנה נתמכת. ייתכן שהתוכנה תהיה גלויה רק ברמת המכשיר גם אם היא אינה נתמכת כעת על-ידי Threat and Vulnerability Management. עם זאת, רק נתונים מוגבלים זמינים.
1. לקבלת שלבים הדוח הדיוק מהפורטל, ראה [אי דיוק בדוח.](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)
   
    **הערה:** דיווח על אי דיוק בפורטל MDE הוא ערוץ 1 ערוצים להנדסה. אם הבעיה דחופה, פתח כרטיס תמיכה.

לקבלת מידע נוסף, [ראה מלאי תוכנה - Threat and Vulnerability Management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).