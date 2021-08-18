---
title: פריסת יישומי Microsoft 365 לארגונים לשימוש משותף ב- RDS , Terminal Server או VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: b8df97c19937a757c1de9865b6c7b8d1cddfd62d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325604"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>פריסת יישומי Microsoft 365 לארגונים לשימוש משותף ב- RDS , Terminal Server או VDI

כדי לפרוס יישומי Microsoft 365 לארגונים באמצעות שירותי שולחן עבודה מרוחק (RDS), שנקרא בעבר שירותי מסוף:

- עליך להיות Microsoft 365 עבור העסק או תוכנית Office 365 הכוללת יישומי Microsoft 365 לארגונים, כגון Office 365 Enterprise E3 או Enterprise E5.
   **הערה:** התוכניות יישומי Microsoft 365 לעסקים והתוכניות Microsoft 365 Business Standard כוללים את יישומי Microsoft 365 לארגונים.
- עליך להפוך הפעלת [מחשב משותפת לזמינה.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

**הערה:** באפשרותך גם להוריד ולהפעיל את [Microsoft מסייע התמיכה והשחזור כדי](https://aka.ms/SaRA_OfficeSCA_M365Portal) להתקין יישומי Microsoft 365 לארגונים במצב הפעלת מחשב משותף.

לקבלת מידע נוסף אודות דרישות מוקדמות, הוראות הגדרה והדרכה לגבי התקנות מותאמות אישית באמצעות כלי הפריסה של Office, ראה [פריסת יישומי Microsoft 365 לארגונים באמצעות שירותי שולחן עבודה מרוחק.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)

כדי לתקן שגיאות הקשורות להפעלת מחשב משותף:

- ראה [פתרון בעיות בהפעלת מחשב משותפת עבור יישומי Microsoft 365 לארגונים.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
- ראה [איפוס יישומי Microsoft 365 עבור מצב הפעלה ארגונית](https://go.microsoft.com/fwlink/?linkid=2109218).

אם ברצונך להתקין את יישומי Microsoft 365 לארגונים ב- RDS מתוך מרכז הניהול של Microsoft 365, המשתמש בהגדרות ***ההתקנה המהוות ברירת מחדל,*** בצע את השלבים הבאים:

1. בדוק איזה מנוי יש לך. [למד כיצד לעשות זאת](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. במקרה הצורך, עבור למנוי אחר. [למד כיצד לעשות זאת](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. אם Office כבר מותקן בשרת RDS באמצעות מנויי Microsoft אחרים, הסר את התקנתו. לדוגמה, על-ידי עבור **אל לוח הבקרה הסר** התקנת  >  **תוכנית.** הסר את [ההתקנה מסייע התמיכה והשחזור](https://aka.ms/SARA-OfficeUninstall-Alchemy) Microsoft אם אתה נכנס לבעיות.
4. בשרת RDS, היכנס אל מרכז הניהול של Microsoft 365 עם חשבון מנהל המערכת שלך [והתקן את יישומי Microsoft 365 לארגונים.](https://portal.office.com/OLS/MySoftware.aspx)
5. לאחר Office מותקן, אל ***תפתח או*** היכנס ליישומים Office אחרים.
6. בשרת RDS, הפוך הפעלת מחשב משותף לזמינה על-ידי עריכת הרישום על-ידי ביצוע השלבים הבאים:
   1. לחץ באמצעות לחצן העכבר Windows לחצן העכבר הימני בפינה הימנית התחתונה של המסך ובחר **הפעל**. בתיבה פתח, הקלד **regedit**, ולאחר מכן בחר **אישור**.
   2. בחר **כן** כאשר תתבקש לאפשר לעורך הרישום לבצע שינויים במכשיר שלך.
   3. בעורך הרישום, הוסף ערך מחרוזת של **SharedComputerensing** עם הגדרה של 1 תחת HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. בשרת RDS, ***היכנס כמשתמש קצה*** וודא שהפעלת מחשב [משותפת זמינה עבור יישומי Microsoft 365 לארגונים.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
