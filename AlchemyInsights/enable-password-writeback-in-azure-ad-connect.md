---
title: אפשר כתיבת חוזרת של סיסמה ב- Azure AD Connect
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 63304667cce67c48fd8bbeee52ff6d61d033ea38fd8d4c4d96c240847dab2cab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118205"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>אפשר כתיבת חוזרת של סיסמה ב- Azure AD Connect

כדי לאפשר כתיבת חוזרת של איפוס סיסמה בשירות עצמי, תחילה אפשר את אפשרות הכתיבה החוזרת ב- Azure AD Connect. מתוך שרת Azure AD Connect, השלם את השלבים הבאים:

1. היכנס אל שרת Azure AD Connect שלך והתחל את אשף קביעת התצורה של **Azure AD Connect**.
2. בדף **הכניסה**, לחץ על **קבע תצורה**.
3. בדף **משימות נוספות**, בחר **התאם אישית אפשרויות סינכרון** ולאחר מכן לחץ על **הבא**.
4. בדף **התחבר ל- Azure AD**, הזן אישור מנהל מערכת כללי עבור הדייר שלך, ולאחר מכן לחץ על **הבא**.
5. בדפי הסינון **ספריות Connect** ו **תחום/OU**, לחץ על **הבא**.
6. בדף **תכונות אופציונליות**, בחר את התיבה לצד **כתיבת חוזרת של סיסמה** ולחץ על **הבא**.
7. בדף **מוכן לקבוע תצורה** לחץ על **קבע תצורה** והמתן שהתהליך יסתיים.
8. כשתראה את סיום קביעת התצורה, לחץ על **יציאה**.

כאשר כתיבה חוזרת של סיסמה מופעלת ב- Azure AD Connect, קבע את התצורה של Azure AD SSPR עבור כתיבה חוזרת.  כדי לאפשר כתיבה חוזרת של סיסמה ב- SSPR, השלם את השלבים הבאים:

1. היכנס אל פורטל Azure באמצעות חשבון מנהל המערכת כללי.
2. חפש אחר **Azure Active Directory** ובחר בו, לחץ על **איפוס סיסמה**, לאחר מכן לחץ על **שילוב מקומי**.
3. להגדיר את האפשרות עבור **כתוב חזרה סיסמאות לספריה המקומית שלך?** על **כן**.
4. להגדיר את האפשרות עבור **אפשר למשתמשים לבטל נעילה של חשבונות מבלי לאפס את הסיסמה שלהם?** ל **כן**.
5. כשתהיה מוכן, לחץ על **שמור**.

לקבלת מידע נוסף, ראה [אפשר כתיבה לאחור לאיפוס סיסמה בשירות עצמי של Azure Active Directory לסביבה מקומית](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).

> [!NOTE]
>  כאשר מנהל מערכת מאפס סיסמה של משתמש בפורטל Azure, אם אותו משתמש מפוקח או שה- hash של הסיסמה מסונכרן, הסיסמה נכתבת לאחור למקומי. פונקציונליות זו דורשת רישיון Azure Premium (‏P1 או P2) והיא אינה נתמכת בשלב זה בפורטל הניהול של Office.
