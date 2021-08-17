---
title: פתרון בעיות SSPR
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
ms.openlocfilehash: 9d8184efdc60befd359059c62ea3eb1a14ad7d2a20dade921d4a71e424f52033
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038959"
---
# <a name="troubleshoot-sspr"></a>פתרון בעיות SSPR

**אני נתקל בבעיות בקביעת התצורה של איפוס סיסמה**

- אם אתה מנהל מערכת ומחפש כיצד לאפשר איפוס סיסמה בשירות עצמי, ראה ערכת לימוד המאפשרת [SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), כדי לקבוע את תצורת איפוס הסיסמה עבור הארגון שלך. ייתכן שתרצה גם לסקור [את דרישות הרישוי.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) בארגון שלך חייב להיות רשיון אחד לפחות.
    - **משתמשים בענן בלבד** - כל Office 365 (O365) בתשלום, או Azure AD Basic
    - **משתמשים בענן ו/או** משתמשים מקומיים - Azure AD Premium P1 או P2, Enterprise Mobility + Security (EMS) או Secure Productive Enterprise (SPE)
- לקבלת שאלות נוספות אודות איפוס סיסמה בשירות עצמי, עיין בשאלות [הנפוצות שלנו.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**אני מקבל הודעת שגיאה**

סקור מאמר זה כדי למצוא שגיאות נפוצות ואת הפתרונות שלהן: [פתרון בעיות של איפוס סיסמה בשירות עצמי](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**אני נתקל בבעיה במדיניות איפוס הסיסמה שלי**

- אם מדיניות איפוס הסיסמה שלך אינה מתנהגת כצפוי, או אם יש לך שאלות לגבי מדיניות איפוס סיסמה, עיין במאמר זה: מדיניות סיסמה [והגבלות ב- Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).
- מדיניות איפוס סיסמה אינה חלה על מנהלי מערכת. Microsoft אוכפת מדיניות חזקה של איפוס סיסמה דו-שערית המהווה ברירת מחדל עבור כל תפקיד מנהל מערכת של Azure. ודא שאתה בודק עם משתמש שהוא אינו מנהל מערכת. לקבלת מידע נוסף אודות מדיניות איפוס מנהל המערכת, עיין במאמר זה: [הבדלי מדיניות איפוס של מנהל מערכת.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)

**איני מעוניין שהמשתמשים שלי ירשמו פרטי אבטחה נוספים לאיפוס סיסמה**

באפשרותך לאכלס מראש נתונים (תכונות דואר אלקטרוני וטלפון) עבור המשתמשים שלך באמצעות API, PowerShell או Azure AD התחברות. כדי ללמוד כיצד לקרוא:

- [פריסת איפוס סיסמה מבלי לדרוש ממשתמשים להירשם](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [אילו נתונים משמשים את איפוס הסיסמה](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**אני רוצה שהמשתמשים שלי ירשמו את פרטי האבטחה הנוספות שלהם לאיפוס סיסמה**

1. האם המשתמשים שלך ירשמו את פרטי האבטחה שלהם לאיפוס סיסמה בשירות עצמי על-ידי [הנחיות aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).
1. לאחר אכלוס הנתונים עבור המשתמש (על-ידי המשתמש או על-ידי מנהל המערכת), [כוון](https://passwordreset.microsoftonline.com/) את המשתמש שלך aka.ms/sspr כך שהמשתמשים שלך יוכלו להיות מורשים לאפס את הסיסמאות שלהם.
1. אם המשתמשים עדיין נתקלים בבעיות, סביר ביותר שהם **מאוחדים או** משתמשים המסונכרנות באמצעות **Hash באמצעות** סיסמה. משמעות הדבר היא ש סביר שיש בעיה בשירות Password Writeback.