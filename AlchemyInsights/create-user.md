---
title: יצירת משתמש
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: a144b172787563b1aa57bdec790df1805a13f078
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323287"
---
# <a name="create-user"></a>יצירת משתמש

**הודעה:**

- [פחת של תמיכת הכניסה של WebView מ- Google החל מ- 4 בינואר 2021.](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) בדוק אם האפליקציות שלך עשויות להיות מושפעות על-ידי [ביצוע ההנחיות של Google](https://go.microsoft.com/fwlink/?linkid=2157323) לגבי תאימות הבדיקה.
- הקפד להשתמש בחוות האינטרנט של המערכת או בדפדפן המערכת בעת כניסה למשתמשים באמצעות חשבונות Google לצרכן. לקבלת מידע נוסף, [ראה בעיות בכניסה ליישום באמצעות דפדפן Chrome בלבד](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).

**איני יכול ליצור משתמש חדש במדריך הכתובות של Azure AD**

1. ודא שאתה מורשה ליצור משתמש רגיל חדש. רק תפקיד מנהל המערכת הכללי או מנהל המשתמשים ב- Azure Active Directory (AD) יכול ליצור משתמש רגיל חדש. אם אינך נמצא באחד התפקידים הללו, בקש ממנהל מערכת להוסיף אותך לאחד התפקידים הללו או ליצור את חשבון המשתמש החדש בשבילך.
1. ודא לשם המשתמש נמצא בתחום שאומת ב- Azure AD שלך. אם אין לך שמות תחומים מותאמים אישית מאומתים ב- Azure AD, באפשרותך להשתמש בתחום ההתחלתי של Azure AD, המסתיים ב- *.onmicrosoft.com.
1. ודא משם המשתמש נמצא בתחום שלא מאוחד ל- Azure AD מה- AD המקומי שלך. לא ניתן להוסיף משתמשים בענן עם שמות תחומים מאוחדים מהסביבה המקומית.
1. ודא שלא קיים כבר שם משתמש או איש קשר אחר שברצונך להקצות למשתמש החדש. שמות משתמשים חייבים להיות ייחודיים ברחבי Azure AD.
1. ראה [תפקידים ומנהלי מערכת של Azure AD עבור](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) Azure AD.
1. ראה את [שמות התחומים עבור](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) Azure AD שלך.
1. סקור [יומני ביקורת](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) כדי לראות מידע מפורט יותר אודות משתמש שנוצר לאחרונה או נמחק, כמו מי ביצע את הפעולה ומתי.
1. לקבלת מידע נוסף אודות הוספת משתמשים חדשים, ראה [שימוש בפורטל Azure כדי ליצור משתמש חדש ב- Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-users-create-azure-portal).
1. [תפקידי ניהול של Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles): הרשאות תפקיד מנהל מערכת ב- Azure Active Directory
1. באפשרותך גם להשתמש [ב- Azure AD PowerShell כדי ליצור משתמש חדש.](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
