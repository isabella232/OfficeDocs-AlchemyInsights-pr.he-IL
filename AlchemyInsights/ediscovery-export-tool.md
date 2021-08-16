---
title: כלי ייצוא גילוי אלקטרוני
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: f7b7e1ae4f1f686fa510403d398c4ff750dbadb9065b8d63701a927eeac52d9b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101303"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>לא ניתן להתקין או להפעיל את כלי הייצוא של גילוי אלקטרוני?

אם אינך יכול להתקין או להפעיל את כלי הייצוא של גילוי אלקטרוני כדי להוריד תוצאות חיפוש, בדוק את הדברים הבאים:
  
- המחשב שבו אתה משתמש ייפגש עם דרישות מוקדמות אלה:

  - גירסאות 32 או 64 סיביות של Windows 7 וגירסאות מתקדמות יותר

  - Microsoft .NET Framework 4.7

  - דפדפן נתמך:

  - Microsoft Edge

    או

  - Internet Explorer 10 וגירסאות מתקדמות יותר

    דפדפנים אחרים, כגון Google Chrome ו- Mozilla Firefox אינם נתמכים.

- הארגון שלך יכול להתחבר אל נקודת הקצה ב- Azure, **\* שהיא .blob.core.windows.net** (תו כללי מייצג מזהה ייחודי עבור עבודת הייצוא שלך).

- מוקצה לך תפקיד ייצוא במרכז Microsoft 365 &amp; האבטחה. כברירת מחדל, תפקיד זה מוקצה רק לקבוצת התפקידים של מנהל גילוי אלקטרוני. ראה [הקצאת הרשאות גילוי אלקטרוני](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

לקבלת מידע נוסף, ראה [ייצוא תוצאות חיפוש תוכן](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

אם אתה מייצא יותר מ- 100,000 תיבות דואר, יהיה עליך להשתמש ב- Powershell הבא כדי להוריד את תוצאות הייצוא: ייצוא תוצאות ביותר מתיבות דואר של  [100K](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).