---
title: התקנת משרד בשרת מסוף-לא מורשה
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 5e6a805fb0b41d714ca1cf90e23b8e2daa90f90e
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/26/2019
ms.locfileid: "37205410"
---
# <a name="installing-office-on-a-terminal-server"></a>התקנת Office בשרת מסופים

עבור פריסת Office 365 ProPlus בשרת Windows באמצעות שירותי שולחן עבודה מרוחק (RDS), שנקרא בעבר שירותי מסוף:
  
- דרושה לך תוכנית Office 365 הכוללת את Office 365 ProPlus, כגון Office 365 Enterprise E3 או Enterprise E5. התוכניות של Office 365 Business ו-Office 365 Business Premium אינן כוללות את Office 365 ProPlus.

- עליך להפוך [הפעלת מחשב משותפת](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)לזמינה.

אם ברצונך להתקין את Office 365 ProPlus ב-RDS ממרכז הניהול של Microsoft 365, ***המשתמש בהגדרות ברירת המחדל של ההתקנה***, השתמש בשלבים הבאים.

> [!TIP]
> באפשרותך גם להוריד ולהפעיל את [מסייע התמיכה והשחזור של Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) כדי להתקין את Office 365 proplus במצב משותף של הפעלת מחשב.
  
1. בדוק מה תוכנית Office 365 יש לך. [למד כיצד](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. במקרה הצורך, עבור לתוכנית אחרת של Office 365. [למד כיצד](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. אם Office כבר מותקן בשרת RDS באמצעות כל תוכנית אחרת של Office 365, הסר את התקנתה. לדוגמה, על-ידי הדרך \> ללוח הבקרה הסר תוכנית. הסר [התקנה באמצעות מסייע התמיכה והשחזור של Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) אם אתה נתקל בבעיות.

4. בשרת RDS, היכנס למרכז הניהול של Microsoft 365 עם חשבון מנהל המערכת שלך [והתקן את Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).

5. לאחר התקנת Office, ***אל תפתח או תיכנס*** ליישומי office כלשהם.

6. בשרת RDS, הפעל הפעלה משותפת של המחשב על-ידי עריכת הרישום על-ידי ביצוע השלבים הבאים:

1. לחץ לחיצה ימנית על לחצן Windows בפינה השמאלית התחתונה של המסך ובחר באפשרות הפעלה. בתיבה פתח את, הקלד **regedit**ולאחר מכן בחר באישור.

2. בחר כן כאשר תתבקש לאפשר לעורך הרישום לבצע שינויים במכשיר.

3. בעורך הרישום, הוסף ערך מחרוזת של **רישוי שיתופיות** עם הגדרה של 1 תחת HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. בשרת RDS, ***היכנס כמשתמש קצה*** [וודא שהפעלת מחשב משותף זמינה עבור Office 365 proplus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

לקבלת פרטים נוספים על דרישות מוקדמות, הוראות התקנה והדרכה בהתקנות מותאמות אישית באמצעות כלי הפריסה של Office, עיין [בפריסת office 365 ProPlus באמצעות שירותי שולחן עבודה מרוחק](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
כדי לתקן שגיאות הקשורות להפעלת מחשב משותף, ראה [פתרון בעיות עם הפעלת מחשב משותף עבור Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  