---
title: התקנת Office בשרת מסופים - ללא רשיון
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 7e435df1515878ab4fe935ab8148daee29b8e3820095fc6e49db45de4c6279db
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055159"
---
# <a name="installing-office-on-a-terminal-server"></a>התקנת Office בשרת מסופים

לפריסת יישומי Microsoft 365 לארגונים בשרת Windows מרוחק באמצעות שירותי שולחן עבודה מרוחק (RDS), שנקרא בעבר שירותי מסוף:
  
- עליך להיות מנוי Microsoft 365 הכולל את יישומי Microsoft 365 לארגונים, כגון Office 365 Enterprise E3 או Enterprise E5. תוכניות יישומי Microsoft 365 לעסקים ותוכניות יישומי Microsoft 365 לעסקים Premium לא כוללות יישומי Microsoft 365 לארגונים.

- עליך להפוך הפעלת מחשב [משותפת לזמינה.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

אם ברצונך להתקין את יישומי Microsoft 365 לארגונים ב- RDS מתוך מרכז הניהול של Microsoft 365, המשתמש בהגדרות ההתקנה ***המוגדרות כברירת מחדל,*** בצע את השלבים הבאים.

> [!TIP]
> באפשרותך גם להוריד ולהפעיל את Microsoft [מסייע התמיכה והשחזור כדי](https://aka.ms/SaRA_OfficeSCA_M365Portal) להתקין יישומי Microsoft 365 לארגונים במצב הפעלת מחשב משותף.
  
1. בדוק איזה Microsoft 365 יש לך. [למד כיצד לעשות זאת](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. במקרה הצורך, עבור למנוי Microsoft 365 אחר. [למד כיצד לעשות זאת](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. אם Office כבר מותקן בשרת RDS באמצעות מנויי Microsoft 365 אחרים, הסר את התקנתו. לדוגמה, על-ידי עבור אל לוח הבקרה \> הסר התקנת תוכנית. הסר את [ההתקנה מסייע התמיכה והשחזור](https://aka.ms/SARA-OfficeUninstall-Alchemy) Microsoft אם אתה נכנס לבעיות.

4. בשרת RDS, היכנס אל מרכז הניהול של Microsoft 365 עם חשבון מנהל המערכת שלך [והתקן יישומי Microsoft 365 לארגונים.](https://portal.office.com/OLS/MySoftware.aspx)

5. לאחר Office מותקן, אל ***תפתח או היכנס*** ליישומים Office אחרים.

6. בשרת RDS, הפוך הפעלת מחשב משותף לזמינה על-ידי עריכת הרישום על-ידי ביצוע השלבים הבאים:

1. לחץ באמצעות לחצן Windows לחצן העכבר הימני בפינה הימנית התחתונה של המסך ובחר הפעל. בתיבה פתח, הקלד **regedit** ולאחר מכן בחר אישור.

2. בחר כן כאשר תתבקש לאפשר לעורך הרישום לבצע שינויים במכשיר שלך.

3. בעורך הרישום, הוסף ערך מחרוזת של **SharedComputerensing** עם הגדרה של 1 תחת HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. בשרת RDS, ***היכנס כמשתמש קצה*** וודא [שהפעלת מחשב משותפת זמינה עבור יישומי Microsoft 365 לארגונים.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)

לקבלת פרטים נוספים על דרישות מוקדמות, הוראות הגדרה והדרכה לגבי התקנות מותאמות אישית באמצעות כלי הפריסה של Office, ראה [פריסת יישומי Microsoft 365 לארגונים באמצעות שירותי שולחן עבודה מרוחק.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)
  
כדי לפתור שגיאות הקשורות להפעלת מחשב משותף, ראה פתרון [בעיות בהפעלת מחשב משותפת עבור יישומי Microsoft 365 לארגונים.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
  