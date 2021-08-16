---
title: פריסת תוספות עבור יישומי Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: 3aacc3c6675f4102a5b34a435c862215dbfd0479b75549d608ed3c91021ed3d7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031407"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>פריסת תוספות עבור יישומי Microsoft 365

פריסה מרכזית היא הדרך המומלצת לפריסת תוספות Office למשתמשים ולקבוצות בארגון שלך. כדי לפרוס תוספות, בצע את השלבים הבאים:

**הערה:** כדי להתקין תוספות עבור Office כמשתמש בודד, ראה [הצגה, ניהול](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)והתקנה של תוספות בתוכניות Office אחרות. כמו כן, ודא שרכישה Office של תוספות של חנות Office זמינה. לקבלת פרטים, ראה [מניעת הורדות תוספת על-ידי כיבוי Office בכל](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)הלקוחות (למעט Outlook) .

1. ודא שהסביבה שלך מותאמת לדרישות לפריסה של תוספות באמצעות פריסה מרכזית. לקבלת פרטים, [ראה דרישות](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).
2. עבור **אל הגדרות**  >    >  **משולבים קבל** אפליקציות מרכז הניהול של Microsoft 365 כדי לפרוס תוספות. 

הערות: 

- אפליקציות משולבות דורשות של למנהל המערכת יש הרשאות מנהל מערכת כללי Exchange מנהל מערכת.

- בעת פריסת תוספות למשתמשים מרובים, מומלץ לבצע מטלות באמצעות קבוצות במקום משתמשים בודדים. לקבלת פרטים, [ראה שיקולים בעת הקצאת תוספת למשתמשים ולקבוצות](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).

- פריסה מרכזית אינה תומכת במשתמשים בקבוצות מקוננות או בקבוצות עם קבוצות אב. לקבלת פרטים, ראה [מטלות משתמשים וקיבוץ](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).

- ודא ששירות Microsoft 365 App Management (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') זמין עבור משתמשים להיכנס. לקבלת פרטים, ראה [קביעת תצורה של מאפייני יישום](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).

- אם אתה נתקל בבעיות בפריסת תוספות באמצעות יישומים משולבים, נסה לפרוס [באמצעות תוספות](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).

לקבלת מידע נוסף, ראה:

[פריסת תוספות במרכז הניהול](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [ניהול תוספות במרכז הניהול](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [שימוש ברכיבי ה- cmdlet של PowerShell](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) בפריסה מרכזית לניהול תוספות 
 [פרסום Office תוספות באמצעות פריסה מרכזית באמצעות מרכז הניהול של Microsoft 365](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [פתרון בעיות: המשתמש אינו רואה תוספות](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [פתרון בעיות בשגיאות משתמש Office תוספות](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)