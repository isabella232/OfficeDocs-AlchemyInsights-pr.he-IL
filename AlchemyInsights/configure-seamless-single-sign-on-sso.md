---
title: קביעת תצורה של כניסה יחידה חלקה (SSO)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004344"
- "9384"
ms.openlocfilehash: 32790b23547de36cd2864e85ebae67f54ad91707
ms.sourcegitcommit: 309b9f3e6e2ff622f95bb860d337d2c05b7bbe54
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/15/2021
ms.locfileid: "50841539"
---
# <a name="configure-seamless-single-sign-on-sso"></a>קביעת תצורה של כניסה יחידה חלקה (SSO)

**קביעת תצורה של יישומים**

1. עליך לקבל את הערכים מספק היישומים. באפשרותך להזין את הערכים באופן ידני או להעלות קובץ מטה-נתונים כדי לחלץ את ערך השדות.
2. יישומים רבים כבר נקבעו מראש לעבודה עם תכלת לספירה. יישומים אלה מפורטים בגלריה של האפליקציות שניתן לעיין בהן בעת הוספת יישום לדייר המודע של תכלת. [סדרת תחלה](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) מובילים אותך בתהליך.
3. כדי ליצור יישום שאינו מופיע בגלריה, באפשרותך ללחוץ על **+ צור** לחצן יישום משלך ולהעניק שם ליישום שלך.
    - כברירת מחדל, הוא יבחר **לשלב כל יישום אחר שאינך מוצא בגלריה** שהיא האפשרות הנכונה עבור יישומים שאינם בגלריה.
    - לאחר שתלחץ על **צור** לאחר הצבת השם עבור היישום, הוא ייצור יישום ארגוני חדש שאינו מהגלריה.
    - לאחר מכן, באפשרותך לנווט **לכניסה יחידה** תחת **ניהול** יישום זה, ותוכל לראות טכניקות שונות להטמעת היישום בסביבה שלך.

**קביעת התצורה של SSO חלק עבור יישום ספציפי**

עבור היישומים בגלריה, תוכל למצוא הוראות מפורטות, שלב אחר שלב. כדי לגשת לשלבים שבהם באפשרותך לעיין ברשימה של כל ערכות הלימוד של קביעת התצורה של האפליקציה בערכות [הלימוד של האפליקציה SaaS app](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list).

**קביעת התצורה של SSO מבוסס SAML**

1. [תחלה: הגדרת כניסה יחידה מבוססת SAML (SSO) עבור יישום בדייר תכלת Active Directory (תכלת AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso).
2. לקבלת מידע נוסף אודות האפשרות המבוססת על SAML עבור כניסה יחידה, ראה [הבנת הכניסה היחידה מבוססת על SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on).
3. לקבלת מידע נוסף אודות בקשות האימות והתגובות של SAML 2.0 התומכות ב-SAML Active Directory (תכלת לספירה) תומך בSign-On בודד (SSO), ראה [בודד Sign-On protocol](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol).
4. כדי ללמוד כיצד ליצור ולקבוע תצורה של כניסה יחידה מבוססת SAML (SSO) עבור היישום שלך ב-תכלת Active Directory (תכלת לספירה) באמצעות API של Microsoft Graph, ראה [קביעת תצורה של כניסה יחידה מבוססת SAML עבור היישום שלך באמצעות Microsoft GRAPH api](https://docs.microsoft.com/graph/application-saml-sso-configure-api).
5. כדי ללמוד כיצד תכלת AD משתמש בפרוטוקול SAML, ראה [כיצד פלטפורמת הזהות של Microsoft משתמשת בפרוטוקול SAML](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference).

**קביעת תצורה של אסימונים וטענות**

1. [כיצד לבצע: התאמה אישית של טענות שהונפקו באסימון SAML עבור יישומים ארגוניים](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).
2. כדי ללמוד כיצד להגדיר טענות באמצעות PowerShell, ראה [כיצד לבצע: התאמה אישית של טענות הנפלטים באסימונים עבור יישום ספציפי בדייר (תצוגה מקדימה)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. כדי ללמוד כיצד לקבוע את התצורה של טענות אופציונליות, ראה [כיצד לספק טענות אופציונליות ליישום שלך](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. כדי ללמוד כיצד להשתמש בתכונות הרחבה של סכימת מדריך כתובות עבור שליחת נתוני משתמש ליישומים בטענות token, ראה [שימוש בתכונות הרחבה של סכימת מדריך כתובות בתביעות](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. כדי ללמוד כיצד להגדיר אורך חיים של אסימונים, ראה [אורך חיים של אסימונים הניתנים להגדרה בפלטפורמת הזהות של Microsoft (תצוגה מקדימה)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
6. [קביעת תצורה של מדיניות אורך חיים של אסימונים (תצוגה מקדימה)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) -במאמר זה, אנו מטיילים בתרחיש מדיניות משותף שיכול לעזור לך לאכוף כללים חדשים עבור אורך חיים של אסימון. בדוגמה, תלמד כיצד ליצור מדיניות הדורשת מהמשתמשים לאמת בתדירות גבוהה יותר ביישום האינטרנט.

**פתרון בעיות של תצורת SSO**

- לשאלות נפוצות אודות שאלות נפוצות בנושא חלק Sign-On (SSO חלק), ראה [הכניסה היחידה של תכלת Active Directory לחלקה אחת: שאלות נפוצות](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- לקבלת מידע אודות פתרון בעיות בנוגע לבעיות נפוצות בנוגע לאופן הSign-On חלקה של מדריך הכתובות של Active Directory (תכלת לספירה), ראה [פתרון בעיות בכניסה יחידה של כניסה יחידה של Active directory](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso).
