---
title: בעיה באיפוס סיסמה
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: 535b5273d367e24ac45b3f60dbc7b6a2da6a3d9affa5a67499989d19a1904768
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039967"
---
# <a name="problems-resetting-password"></a>בעיות באיפוס סיסמה

להלן כמה מהבעיות שייתכן שתתמודד מולן בעת איפוס הסיסמה והפתרונות האפשריים:

**אני נתקל בבעיה עם איפוס סיסמה שלא מכוסה בקטגוריות האחרות**

- ודא שאתה מורשה לאפס סיסמאות. רק כללי, סיסמה ומנהלי משתמשים יכולים לאפס סיסמאות משתמש. מנהלי מערכת כלליים יכולים גם לאפס סיסמאות של מנהל מערכת בעל הרשאות אחרות.
- ודא שאתה מבין את דרישות הרישוי:
    - חייב להיות לך רשיון אחד לפחות שהוקצה בארגון שלך
        - משתמשים בענן בלבד - כל Office 365 (O365) בתשלום, או Azure AD Basic
        - משתמשים בענן ו/או משתמשים מקומיים - Azure AD Premium P1 או P2, Enterprise Mobility + Security (EMS) או Secure Productive Enterprise (SPE)
        - כדי לקרוא עוד אודות דרישות רישוי, עיין במאמר [דרישות רישוי](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)עבור איפוס סיסמה בשירות עצמי של Azure AD .

**אני נתקל בבעיות בבדיקת מדיניות איפוס הסיסמה שאני מגדיר**

- שכפול של פריטי מדיניות שהוחלו לאחרונה עשוי להימשך כמה דקות בכל מרכזי הנתונים ונקודות הקצה. המרחק הפיזי ממרכז הנתונים ישפיע גם על מהירות החלת השינויים.
- בדוק עם משתמש קצה, לא מנהל מערכת וטייס עם קבוצה קטנה של משתמשים. פריטי המדיניות המוגדרים בפורטל Azure חלים רק על משתמשי קצה, ולא על מנהלי מערכת. Microsoft אוכפת מדיניות חזקה לאיפוס סיסמה דו-שערית המהווה ברירת מחדל עבור כל תפקיד מנהל מערכת של Azure (לדוגמה: מנהל מערכת כללי, מנהל מערכת של Helpdesk, Password Administrator וכדומה)
    - קבל מידע נוסף [על מדיניות עבור מנהלי מערכת](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).

**אני רוצה לפרוס איפוס סיסמה, אך איני מעוניין שהמשתמשים שלי ירשמו פרטי אבטחה נוספים**

אכלוס מראש של נתונים עבור המשתמשים שלך כדי שלא יתו להם! - כמנהל מערכת, באפשרותך להגדיר מאפייני טלפון ודעת דואר אלקטרוני עבור המשתמשים שלך לפני שתאפס את הסיסמה לארגון שלך. באפשרותך לעשות זאת באמצעות API, PowerShell או Azure AD התחברות. מידע נוסף כאן:
- [פריסת איפוס סיסמה מבלי לדרוש ממשתמשים להירשם](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [אילו נתונים משמשים את איפוס הסיסמה](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**לחצן איפוס הסיסמה אפור**

אינך מורשה לאפס את הסיסמאות של משתמש זה. רק כללי, סיסמה ומנהלי משתמשים יכולים לאפס סיסמאות משתמש. מנהלי מערכת כלליים יכולים גם לאפס סיסמאות של מנהל מערכת בעל הרשאות אחרות.

**איני רואה את להב איפוס הסיסמה**

אינך מורשה לאפס סיסמאות. רק כללי, סיסמה ומנהלי משתמשים יכולים לאפס סיסמאות משתמש. מנהלי מערכת כלליים יכולים גם לאפס סיסמאות של מנהל מערכת בעל הרשאות אחרות.

**איני רואה את להב השילוב המקומי באיפוס סיסמה**

- להב השילוב המקומי מופיע רק בסביבות היברידיות - כלומר, אתה משתמש ב- writeback באמצעות סיסמה כדי לטפל בסיסמאות של המשתמש המקומי.
- אינך רואה להב זה אם:
    - אינך משתמש בסיסמה writeback
    - ישנה בעיה בהתקנה/קישוריות של writeback של סיסמה
    - ישנה בעיה בהתקנה/קישוריות של Azure AD התחברות
    - לקבלת שלבים נוספים לפתרון בעיות בכתיבה חוזרת באמצעות סיסמה, עיין בסעיף פתרון [בעיות בכתיבה חוזרת באמצעות סיסמה](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**איני יודע כיצד לאפס סיסמת משתמש**

1. היכנס לפורטל Azure כמנהל מערכת מתאים.
1. עבור אל להב המשתמשים והקבוצות, בחר **כל המשתמשים**.
1. בחר משתמש מהרשימה.
1. עבור המשתמש שנבחר, בחר מבט **כולל** ולאחר מכן, בשורת הפקודות, לחץ על **איפוס סיסמה**.
1. בצע את ההוראות שעל המסך.
    - רק איפוסים שבוצעו באמצעות Writeback של סיסמת התמיכה בפורטל Azure.

**אני מאפס סיסמת משתמש מקומית מתוך פורטל Office 365 Admin או Office 365 למכשירים ניידים, אך המשתמש עדיין אינו יכול להיכנס**

אין תמיכה ב- Password Writeback בפורטל זה. איפוס סיסמת המשתמש שוב בפורטל Azure - portal.azure.com

