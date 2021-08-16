---
title: בעיות עם משאב או מנהל שירות
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
- "9004336"
- "7741"
ms.openlocfilehash: 52b9b2e950d66c2f4105b76c4e2c70ed51320e4a57eb0008c353a9587fcc6510
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028077"
---
# <a name="issues-with-a-resource-or-service-principal"></a>בעיות עם משאב או מנהל שירות

1. אם אתה רק מתחיל בעבודה, אובייקטים ראשיים של יישומים ושירות ב- [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) מתארים רישום יישומים, אובייקטי יישומים ומנהלי שירות ב- Azure Active Directory: מה הם, אופן שימושם ואופן הקשורים זה לזה. תרחיש לדוגמה מרובה דיירים מוצג גם כדי להמחיש את קשר הגומלין בין אובייקט היישום של יישום לאובייקטים ראשיים תואמים של השירות.
2. באפשרותך לקבל מידע נוסף על קשר הגומלין בין יישומים למנהלי שירות על-ידי קריאת [יישומים לאובייקטים ראשיים של שירות ב- Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
3. [כיצד: השתמש בפורטל](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) כדי ליצור יישום ומנהל שירות של Azure AD העשים גישה למשאבים, מראה לך כיצד ליצור יישום חדש של Azure Active Directory (Azure AD) ומנהל שירות, איתם ניתן להשתמש עם פקד הגישה המבוסס על תפקידים.
4. באמצעות [ה- API הראשי של השירות,](https://docs.microsoft.com/graph/api/resources/serviceprincipal)באפשרותך לנהל באופן תיכנותי מופעים של יישומים ולנהל את היישומים שיישומים יכולים לעשות בתוך הדייר שלך.
5. [servicePrincipal resource type מפרט](https://docs.microsoft.com/graph/api/resources/serviceprincipal) את כל המאפיינים והשיטות עבור סוג המשאבPrincipal של השירות.
6. [הבדלים בין סוגי משאבים בין Azure AD Graph לבין Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) מדגיש הבדלים בין Azure AD Graph לבין משאבי Microsoft Graph Microsoft. היא מציגה משאבים עם שמות שונים או אינם זמינים; היא גם מדגישה משאבים הזמינים בגירסת הביתא של Microsoft Graph אך לא בגירסת v1.0.

**בעיות עם משתמשים אורחים**

- [התחלה מהירה: הוספת משתמשים](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) אורחים למדריך הכתובות בפורטל Azure מראה לך כיצד להוסיף משתמש אורח חדש לספריית Azure AD שלך דרך פורטל Azure, לשלוח הזמנה ולראות כיצד נראה תהליך המימוש בהזמנה של המשתמש אורח.
- [ערכת לימוד: יצירת תזרימות משתמשים ב- Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) מראה לך כיצד ליצור זרימה מומלצת של משתמשים באמצעות פורטל Azure. אם אתה מחפש מידע אודות אופן הגדרת זרימת אישורי סיסמת בעלי משאב (ROPC) ביישום שלך, ראה קביעת התצורה של אישורי סיסמת הבעלים של המשאב ב- Azure AD B2C.
