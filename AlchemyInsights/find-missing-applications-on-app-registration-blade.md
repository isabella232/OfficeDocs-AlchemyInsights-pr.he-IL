---
title: חיפוש יישומים חסרים בלהב רישום יישומים
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
- "9004352"
- "9654"
ms.openlocfilehash: 00b5821e2edad8b60ff60b1f85264d81c72277e4
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404694"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>חיפוש יישומים חסרים בלהב רישום יישומים

1. אין אפשרות למצוא יישומים בפורטל רישום יישומים.

    אם יישום הוא יישום מרובה דיירים והוא נרשם דייר אחר, הוא לא יוצג תחת להב רישום יישומים. עם זאת, ייתכן שתמצא אותה תחת להב של יישומים ארגוניים לאחר שהגישה אליו (לאחר הסכמתה) ומנהל השירות נוצר דייר שלך. לקבלת מידע נוסף, ראה [אפליקציות & שירות ב- Azure AD - פלטפורמת הזהויות של Microsoft](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
2. לא ניתן להציג יישומים בלהב רישום יישומים למרות שאתה מנהל מערכת.

    ודא שאתה נמצא במדריך הכתובות הנכון בפורטל Azure.
3. היישום שלי אינו מופיע תחת להב של יישומים ארגוניים, אך הוא מופיע בעת ביצוע שאילתה על הפקודה PowerShell.

    לעתים, לאחר מחיקת היישום מהפורטל Azure, הוא אינו מופיע בפורטל, אך ייתכן שהוא לא נמחק לחלוטין. לקבלת מידע נוסף, ראה:
    - באפשרותך לאחזר את רשימת היישומים שנמחקו בעבר ולראות אם היישום מופיע ברשימה באמצעות הפקודה Powershell: **Get-AzureADDeletedApplication**. כדי ללמוד עוד, [ראה Get-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication).
    - אם ברצונך להסיר את היישום לחלוטין, באפשרותך לנסות את הפעולות הבאות ב- PowerShell: **Remove-AzureADApplication -ObjectId**. כדי ללמוד עוד, ראה [Remove-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication).
    - לחלופין, באפשרותך לנסות לשחזר את היישום שנמחק באמצעות הפקודה הבאה של Powershell: **שחזור AzureADDeletedApplication -ObjectId**. כדי ללמוד עוד, ראה [שחזור-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
4. לא ניתן למצוא רשימה של כל היישומים הארגוניים המותקנים מראש דייר Azure החדש שלי.

    אין יישומים ארגוניים מותקנים מראש ב- Azure AD כברירת מחדל. עליך להוסיף אותו באופן ידני מהאפשרות 'יישום חדש' על-ידי גלישה בו מתוך גלריית Azure AD או הוספת יישום שאינו גלריה. כדי ללמוד עוד, ראה [התחלה מהירה: הוספת יישום לדייר Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    אם אתה מנהל מערכת כללי, באפשרותך לגשת בקלות לאפליקציות שלך באמצעות מפעיל היישומים [של Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher).
5. לא ניתן למצוא את האפליקציות שלי בפורטל 'היישומים שלי'.

    ודא שיישומים אינם מוסתרים בדף אוסף היישומים שלי. כדי ללמוד עוד, ראה [אוספים (תצוגה מקדימה) בפורטל היישומים שלי - Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections).
6. כדי להפעיל אפליקציות מהפורטל 'היישומים שלי', ראה איתור & שימוש [באפליקציות בפורטל 'היישומים שלי' - Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access).
7. אפליקציית Office 365 Mover אינה מופיעה בלהב של יישומים ארגוניים לאחר ההתקנה.

    היישום 'Office 365 Mover' הוא יישום רב-משתתפים שאין צורך להוסיף אותו ל- AAD באמצעות המקטע 'יישומי גלריה' תחת רישום יישומים ארגוניים. כדי לגשת לאפליקציה Office 365 Mover, פשוט היכנס לאפליקציה ותבקש את הסכמת המשתמש עבור ההרשאות. לאחר שהמשתמש מספק את ההסכמה, יישום זה יתווסף באופן אוטומטי לדייר עם מזהה הדואר האלקטרוני שנכנסת.

    לאחר הכניסה ליישום, תוכל למצוא את הערך של יישום זה תחת הלהב של היישומים הארגוניים ב- AAD. עליך לחפש יישום זה על-ידי הקלדת השם המלא, כלומר "Office 365 Mover" או פשוט חפש "office" ועליה רשימת האפליקציה. כדי ללמוד עוד, ראה [Office 365 Mover](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)אומר שהוא כבר מותקן, אך הוא אינו מופיע בגלריית היישומים הארגוניים .
8. התחלה מהירה: הצג את רשימת היישומים המשתמשים דייר [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) לניהול זהויות מראה לך כיצד להציג את היישומים, הידועים גם כאפליקציות, שכבר מוגדרים לשימוש דייר Azure AD כספק הזהויות (IdP).
9. [פתרון בעיות נפוצות בהוספה או הסרה של יישום ל- Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) עוזר לך להבין את הבעיות הנפוצות שאנשים צופים אפליקציות ב- Azure Active Directory.
