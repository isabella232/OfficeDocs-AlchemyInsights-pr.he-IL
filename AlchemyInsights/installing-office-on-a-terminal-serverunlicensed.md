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
ms.openlocfilehash: 35ef317ea87fedd01c08fee5b370e3c81e515c27
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322000"
---
# <a name="installing-office-on-a-terminal-server"></a>התקנת Office בשרת מסופים

לפריסת יישומי Microsoft 365 לארגונים בשרת Windows מרוחק באמצעות שירותי שולחן עבודה מרוחק (RDS), שנקרא בעבר שירותי מסוף:
  
- עליך להיות מנוי Microsoft 365 הכולל את יישומי Microsoft 365 לארגונים, כגון Office 365 Enterprise E3 או Enterprise E5. תוכניות יישומי Microsoft 365 לעסקים ותוכניות יישומי Microsoft 365 לעסקים Premium לא כוללות יישומי Microsoft 365 לארגונים.

- עליך להפוך הפעלת מחשב [משותפת לזמינה.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

אם ברצונך להתקין את יישומי Microsoft 365 לארגונים ב- RDS מתוך מרכז הניהול של Microsoft 365, המשתמש בהגדרות ההתקנה ***המוגדרות כברירת מחדל,*** בצע את השלבים הבאים.

    **Tip**: You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.
  
1. בדוק איזה Microsoft 365 יש לך. [למד כיצד לעשות זאת](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. במקרה הצורך, עבור למנוי Microsoft 365 אחר. [למד כיצד לעשות זאת](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. אם Office כבר מותקן בשרת RDS באמצעות מנויי Microsoft 365 אחרים, הסר את התקנתו. לדוגמה, על-ידי עבור אל לוח הבקרה \> הסר התקנת תוכנית. הסר את [ההתקנה מסייע התמיכה והשחזור](https://aka.ms/SARA-OfficeUninstall-Alchemy) Microsoft אם אתה נכנס לבעיות.

4. בשרת RDS, היכנס אל מרכז הניהול של Microsoft 365 עם חשבון מנהל המערכת שלך [והתקן את יישומי Microsoft 365 לארגונים.](https://portal.office.com/OLS/MySoftware.aspx)

5. לאחר Office, אל ***תפתח*** או היכנס ליישומים Office אחרים.

6. בשרת RDS, הפוך הפעלת מחשב משותף לזמינה על-ידי עריכת הרישום על-ידי ביצוע השלבים הבאים:

1. לחץ באמצעות לחצן Windows הימני בפינה הימנית התחתונה של המסך ובחר הפעל. בתיבה פתח, הקלד **regedit** ולאחר מכן בחר אישור.

2. בחר כן כאשר תתבקש לאפשר לעורך הרישום לבצע שינויים במכשיר שלך.

3. בעורך הרישום, הוסף ערך מחרוזת של **SharedComputerensing** עם הגדרה של 1 תחת HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. בשרת RDS, ***היכנס כמשתמש קצה*** וודא שהפעלת מחשב [משותפת זמינה עבור יישומי Microsoft 365 לארגונים.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)

לקבלת פרטים נוספים על דרישות מוקדמות, הוראות הגדרה והדרכה לגבי התקנות מותאמות אישית באמצעות כלי הפריסה של Office, ראה [פריסת יישומי Microsoft 365 לארגונים באמצעות שירותי שולחן עבודה מרוחק.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)
  
כדי לפתור שגיאות הקשורות להפעלת מחשב משותף, ראה פתרון [בעיות בהפעלת מחשב משותפת עבור יישומי Microsoft 365 לארגונים.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
  