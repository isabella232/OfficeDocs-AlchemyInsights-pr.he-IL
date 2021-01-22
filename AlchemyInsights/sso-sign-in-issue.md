---
title: בעיות כניסה חלקה של SSO user
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935124"
---
# <a name="seamless-sso-user-sign-in-issues"></a>בעיות כניסה חלקה של SSO user

לאחר שהמשתמש מאומת, הדפדפן יאחסן במטמון את אישורי המשתמש, כך שאותו דפדפן, היישום ייכנס באופן אוטומטי באמצעות אותו חשבון. פעולה זו עשויה להקשות על משתמש אחר או על משתמש בודד להיכנס לחשבונות מרובים במכשיר אחד. כדי לפתור את הבעיה: 1. נסה להיכנס לדפדפן אחר. 2. נקה את המטמון ו/או את קבצי ה-cookie של הדפדפן ונסה להיכנס שוב.

אם אתה עדיין נתקל בבעיות כניסה, מומלץ לבצע את הפעולות הבאות כדי לאבחן ולהפוך את שלבי הפתרון:

1. התקן את [ההרחבה ' היישומים שלי ' מאובטח בדפדפן](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) כדי לעזור לתכלת Active Directory (תכלת לספירה) כדי לספק אבחנה ופתרונות טובים יותר בעת שימוש בחוויית הבדיקה בפורטל התכלת.
2. לשחזר את השגיאה באמצעות חוויית הבדיקה בדף קביעת התצורה של האפליקציה בפורטל תכלת. לקבלת מידע נוסף, ראה [יישומי כניסה יחידה המבוססים על SAML של Debug](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues).
3. אם אתה משתמש בחוויית הבדיקה בפורטל ' תכלת ' עם הרחבת הדפדפן ' היישומים שלי ' מאובטחת, באפשרותך **לדלג על שלב 4**.
4. כדי לפתוח את הדף תצורת כניסה יחידה מבוססת SAML:
    - פתח את [פורטל התכלת](https://portal.azure.com/) והיכנס **כמנהל מערכת כללי** או **כCoadmin**.
    - פתח את **ההרחבה תכלת Active Directory** על-ידי בחירת **כל השירותים** בחלק העליון של תפריט הניווט הראשי בצד הימני.
    - הקלד "תכלת Active Directory" בתיבת החיפוש filter ובחר את הפריט **תכלת Active directory** .
    - בחר באפשרות **יישומים ארגוניים** מתפריט הניווט הימני של תכלת של active Directory.
    - בחר **את כל היישומים** כדי להציג רשימה של כל היישומים שלך. אם אינך רואה את היישום שברצונך להציג כאן, השתמש בפקד **המסנן** בחלק העליון של **הרשימה כל היישומים** והגדר את האפשרות **הצג** לכל **היישומים**.
    - בחר את היישום שברצונך לקבוע את תצורתו עבור כניסה יחידה.
    - לאחר הטעינה של היישום, בחר **כניסה יחידה** מתפריט הניווט הימני של היישום.
    - בחר **SSO מבוסס SAML**.
5. בהתבסס על השגיאה, כדי לקבל מידע נוסף על השלבים המומלצים שעליך לעקוב אחריהם, ראה [בעיות בכניסה ליישומים המוגדרים כניסה יחידה מבוססת SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory).
6. כדי לפתור בעיות אחרות בחתימת משתמשים, עיין בהנחיות הבאות:
    - [פרוטוקול SAML בודד Sign-On](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [כיצד לבצע: פתרון שגיאות כניסה באמצעות הדוחות הפעילים של Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [בקשה להסכמה בלתי צפויה](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [שגיאת הסכמה למשתמש](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [בעיות בכניסה מהיישומים שלי](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [שגיאה בעמוד כניסה ליישום](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [בעיה בכניסה ליישום Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
