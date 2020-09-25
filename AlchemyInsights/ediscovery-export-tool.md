---
title: כלי הייצוא של גילוי אלקטרוני
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277933"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>לא ניתן להתקין או להפעיל את כלי הייצוא של גילוי אלקטרוני?

אם אינך מצליח להתקין או להפעיל את כלי הייצוא של גילוי אלקטרוני כדי להוריד תוצאות חיפוש, בדוק את הדברים הבאים:
  
- המחשב שבו אתה משתמש עומד בדרישות הדרישות המוקדמות הבאות:

  - גירסאות 32 או 64 סיביות של Windows 7 וגירסאות מתקדמות יותר

  - Microsoft .NET Framework 4.7

  - דפדפן נתמך:

  - מייקרוסופט אדג'

    או

  - Internet Explorer 10 וגירסאות מתקדמות יותר

    דפדפנים אחרים, כגון Google Chrome ו-Mozilla Firefox אינם נתמכים.

- הארגון שלך יכול להתחבר לנקודת הקצה בתכלת, שהיא ** \* . blob.core.windows.net** (התווים הכלליים מייצגים מזהה ייחודי עבור משימת הייצוא שלך).

- מוקצית לך תפקיד הייצוא במרכז תאימות האבטחה של Microsoft 365 &amp; . כברירת מחדל, תפקיד זה מוקצה רק לקבוצת התפקידים של גילוי אלקטרוני Manager. ראה [הקצאת הרשאות גילוי אלקטרוני](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

לקבלת מידע נוסף, ראה [ייצוא תוצאות חיפוש תוכן](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

אם אתה מייצא יותר מ-100 תיבות דואר, יהיה עליך להשתמש ב-Powershell הבאים כדי להוריד את תוצאות הייצוא:  [ייצוא תוצאות של יותר מ-100 תיבות דואר](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).