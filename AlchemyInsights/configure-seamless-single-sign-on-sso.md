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
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: bd3873c2db1b8d548f81d531a8bf5747130fe761
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402268"
---
# <a name="configure-seamless-single-sign-on-sso"></a>קביעת תצורה של כניסה יחידה חלקה (SSO)

**קביעת תצורה של יישומים**

1. עליך לקבל את הערכים מספק היישום. באפשרותך להזין את הערכים באופן ידני או להעלות קובץ מטה-נתונים כדי לחלץ את ערך השדות.
2. אפליקציות רבות כבר הוגדרה מראש לעבודה עם Azure AD. אפליקציות אלה מפורטות בגלריית היישומים ש באפשרותך לעיין בהם בעת הוספת יישום לדייר Azure AD שלך. הסידרה ['התחלה מהירה'](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) תסדר אותך לאורך התהליך.
3. כדי ליצור יישום שאינו גלריה, באפשרותך ללחוץ **על + צור לחצן יישום** משלך ולתן שם ליישום שלך.
    - כברירת מחדל, הוא **יבחר** שילוב כל יישום אחר שלא תמצא בגלריה, שהיא האפשרות הנכונה עבור יישומים שאינם גלריה.
    - לאחר שתכה **צור** לאחר שתציב את השם עבור היישום, הוא ייצור יישום ארגוני חדש שאינו גלריה.
    - לאחר מכן, תוכל לנווט אל  **כניסה** יחידה תחת ניהול של יישום זה, ואתה תוכל לראות טכניקות שונות ליישום שלו בסביבה שלך.

**קביעת תצורה של SSO חלק עבור יישום ספציפי**

עבור האפליקציות בגלריה תמצא הוראות מפורטות, שלב אחר שלב. כדי לגשת לשלבים, באפשרותך לעיין ברשימה של כל ערכות הלימוד של קביעת התצורה של האפליקציה בערכות [הלימוד של קביעת התצורה של האפליקציה SaaS](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list).

**קביעת תצורה של SSO מבוסס SAML**

1. [התחלה מהירה: הגדרת כניסה יחידה מבוססת SAML (SSO)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)עבור יישום דייר Azure Active Directory (Azure AD).
2. לקבלת מידע נוסף על האפשרות מבוססת SAML עבור כניסה יחידה, ראה הבנת כניסה יחידה מבוססת [SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on).
3. כדי ללמוד אודות בקשות האימות והתגובות של SAML 2.0 התומכות ב- Azure Active Directory (Azure AD) ב- single Sign-On (SSO), [ראה פרוטוקול SAML Sign-On יחיד .](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
4. כדי ללמוד כיצד ליצור ולהגדיר כניסה יחידה מבוססת SAML (SSO) עבור היישום שלך ב- Azure Active Directory (Azure AD) באמצעות ה- API של Microsoft Graph, ראה קביעת תצורה של כניסה יחידה מבוססת SAML עבור היישום שלך באמצעות [ה- API של Microsoft Graph](https://docs.microsoft.com/graph/application-saml-sso-configure-api).
5. כדי ללמוד כיצד Azure AD משתמש בפרוטוקול SAML, ראה [כיצד פלטפורמת הזהויות של Microsoft משתמשת בפרוטוקול SAML](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference).

**קביעת תצורה של אסימונים ותביעות**

1. [כיצד לבצע: התאמה אישית של תביעות שהונפקו באסימון SAML עבור יישומים ארגוניים](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).
2. כדי ללמוד כיצד לקבוע את התצורה של תביעות באמצעות PowerShell, ראה כיצד לבצע: התאמה אישית של תביעות שהופצו באסימונים עבור [יישום ספציפי דייר (תצוגה מקדימה)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. כדי ללמוד כיצד לקבוע תצורה של תביעות אופציונליות, [ראה כיצד: מתן תביעות אופציונליות לאפליקציה שלך](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. כדי ללמוד כיצד להשתמש בתכונות הרחבת סכימת מדריך כתובות לשליחת נתוני משתמשים ליישומים בתביעות אסימון, ראה [שימוש בתכונות הרחבת סכימת מדריך כתובות בתביעות](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. כדי ללמוד כיצד לקבוע תצורה של משך חיים של אסימון, ראה משך חיים של אסימון [הניתן להגדרה בפלטפורמות הזהויות של Microsoft (תצוגה מקדימה)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
6. [קביעת תצורה של מדיניות משך חיים של אסימון (תצוגה מקדימה)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) - במאמר זה, אנו עוברים על תרחיש מדיניות משותף שיסייע לך לכפות כללים חדשים עבור משך חיים של אסימון. בדוגמה, תלמד כיצד ליצור מדיניות שדורשת מהמשתמשים לבצע אימות בתדירות גבוהה יותר באפליקציית האינטרנט שלך.

**פתרון בעיות בתצורת SSO**

- לקבלת שאלות נפוצות אודות Azure Active Directory Seamless Single Sign-On (חלקה SSO), ראה כניסה יחידה חלקה של [Azure Active Directory: שאלות נפוצות.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)
- לקבלת מידע לפתרון בעיות נפוצות לגבי Azure Active Directory (Azure AD) חלקה יחידה Sign-On (SSO חלקה), ראה פתרון בעיות ב- Azure Active Directory Seamless Single [Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso).
