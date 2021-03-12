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
ms.openlocfilehash: 742ff857141d08031302fdcff7e49b3eef90e0f7
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744974"
---
# <a name="create-user"></a>יצירת משתמש

**ודעה**

- [תבטלות של תמיכה בכניסה של תצוגת האינטרנט מ-Google החל מ-4 בינואר 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) . בדיקה אם היישומים שלך עשויים להיות מושפעים על-ידי ביצוע [ההדרכה של Google](https://go.microsoft.com/fwlink/?linkid=2157323) לגבי תאימות בדיקות.
- הקפד להשתמש בתצוגת האינטרנט של המערכת או בדפדפן המערכת בעת הכניסה למשתמשים שלך באמצעות חשבונות של Google לצרכן. לקבלת מידע נוסף, ראה [בעיות בכניסה ליישומים באמצעות דפדפן Chrome בלבד](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).

**איני מצליח ליצור משתמש חדש במדריך הכתובות של תכלת**

1. ודא שאתה מורשה ליצור משתמש רגיל חדש. רק התפקיד ' מנהל מערכת כללי ' או ' מנהל משתמשים ' ב-תכלת Active Directory (AD) יכול ליצור משתמש רגיל חדש. אם אינך נמצא באחד מתפקידים אלה, בקש ממנהל מערכת להוסיף אותך לאחד מתפקידים אלה או כדי ליצור את חשבון המשתמש החדש עבורך.
1. ודא ששם המשתמש נמצא בתחום שאומת במודעת התכלת. אם אין לך שמות תחומים מותאמים אישית מאומתים במודעת התכלת שלך, באפשרותך להשתמש בתחום הראשוני של המודעה של תכלת, שמסתיים ב-*. onmicrosoft.com.
1. ודא ששם המשתמש נמצא בתחום שאינו מאוחד לתכלת לספירה מהמודעה המקומית שלך. לא ניתן להוסיף משתמשים בענן באמצעות שמות תחומים המאוחדים מקומיים.
1. ודא שאין למשתמש או איש קשר אחר כבר את שם המשתמש שברצונך להקצות למשתמש החדש. שמות משתמשים חייבים להיות ייחודיים בין תכלת לספירה.
1. ראה [תפקידים ומנהלי מערכת של ' תכלת '](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) עבור הודעת התכלת.
1. ראה את [שמות התחומים](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) עבור הודעת התכלת.
1. סקור [יומני ביקורת](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) כדי לראות מידע מפורט יותר אודות משתמש שנוצר או נמחק לאחרונה, כגון מי שביצע את הפעולה ומתי.
1. לקבלת מידע נוסף אודות הוספת משתמשים חדשים, ראה [שימוש בפורטל ' תכלת ' כדי ליצור משתמש חדש במודעת התכלת](/azure/active-directory/active-directory-users-create-azure-portal).
1. [תפקידים מנהליים של תכלת לספירה](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles): הרשאות תפקיד מנהל מערכת ב-תכלת active Directory
1. [באפשרותך גם להשתמש ב-תכולים AD PowerShell כדי ליצור משתמש חדש](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).
