---
title: פתרון בעיות ב-SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429719"
---
# <a name="troubleshoot-sspr"></a>פתרון בעיות ב-SSPR

**אני נתקל בבעיות בקביעת התצורה של איפוס סיסמה**

- אם אתה מנהל מערכת ומחפש כיצד להפוך איפוס סיסמה בשירות עצמי לזמין, ראה [ערכת לימוד הפעלת SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), כדי לקבוע את התצורה של איפוס סיסמה עבור הארגון שלך. ייתכן שתרצה גם לסקור את [דרישות הרישוי](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support). דרוש לך רשיון אחד לפחות המוקצה לארגון שלך.
    - **משתמשים בענן בלבד** -כל אחד מהמשתמשים של Office 365 (O365) שילם SKU או תכלת AD Basic
    - **משתמשים בענן ו/או מקומיים** -תכלת AD P1 או P2, ניידות ארגונית + אבטחה (EMS), או מאובטח של ארגון פרודוקטיבי (מהירות)
- לקבלת שאלות נוספות אודות איפוס סיסמה בשירות עצמי, עיין בשאלות [הנפוצות שלנו](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).

**אני מקבל הודעת שגיאה**

עיין במאמר זה כדי לאתר שגיאות נפוצות והפתרונות שלהן: [פתרון בעיות באיפוס סיסמה בשירות עצמי](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**אני נתקל בבעיה במדיניות ' איפוס הסיסמה שלי '**

- אם מדיניות איפוס הסיסמאות אינה מתנהגת כמצופה, או אם יש לך שאלות לגבי מדיניות איפוס סיסמה, עיין [במאמר זה: מדיניות סיסמה והגבלות ב-תכלת Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- מדיניות איפוס סיסמאות אינה חלה על מנהלי מערכת. Microsoft אוכפת מדיניות ברירת מחדל מסוג ברירת מחדל לאיפוס סיסמה עבור כל תפקיד מנהל מערכת של תכלת. ודא שאתה בוחן עם משתמש שאינו מנהל מערכת. לקבלת מידע נוסף אודות מדיניות איפוס מנהל מערכת, עיין במאמר זה: [איפוס הבדלי מדיניות של מנהל מערכת](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).

**איני מעוניין שהמשתמשים יוכלו לרשום פרטי אבטחה נוספים עבור איפוס סיסמה**

באפשרותך לאכלס מראש נתונים (דואר אלקטרוני ותכונות טלפון) עבור המשתמשים שלך באמצעות מחבר API, PowerShell או תכלת לספירה. כדי ללמוד כיצד לקרוא:

- [פריסת איפוס סיסמה מבלי לחייב משתמשים לרשום](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [אילו נתונים משמשים לאיפוס סיסמה](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**אני מעוניין שהמשתמשים שלי ירשמו את פרטי האבטחה הנוספים שלהם לאיפוס סיסמה**

1. בקש מהמשתמשים לרשום את מידע האבטחה שלהם עבור איפוס סיסמה בשירות עצמי על-ידי הפניית הקישור אל [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).
1. לאחר שהנתונים מאוכלסים עבור המשתמש (על-ידי המשתמש או על-ידי מנהל המערכת), הפנה את המשתמש שלך ל- [aka.ms/sspr](https://passwordreset.microsoftonline.com/) כדי שהמשתמשים יוכלו להיות מוסמכים כדי לאפס את הסיסמאות שלהם.
1. אם המשתמשים עדיין חווים בעיות, הם ככל הנראה משתמשים מסונכרנים ב-hash **מאוחדים** או **בסיסמאות** . משמעות הדבר היא שסביר להניח שקיימת בעיה בשירות Password Writeback.