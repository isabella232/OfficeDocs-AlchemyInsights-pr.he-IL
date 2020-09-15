---
title: התקנת office בשרת מסוף-לא מורשה
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
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663118"
---
# <a name="installing-office-on-a-terminal-server"></a>התקנת Office בשרת מסופים

לפריסת יישומי Microsoft 365 עבור enterprise בשרת Windows באמצעות שירותי שולחן עבודה מרוחק (RDS), שנקראו בעבר ' שירותי מסוף ':
  
- דרוש לך מנוי של Microsoft 365 הכולל יישומי Microsoft 365 עבור enterprise, כגון Office 365 Enterprise E3 או Enterprise E5. האפליקציות של Microsoft 365 לעסקים ו-Microsoft 365 Apps עבור business Premium אינן כוללות אפליקציות של Microsoft 365 עבור enterprise.

- עליך להפוך [הפעלת מחשב משותפת](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)לזמינה.

אם ברצונך להתקין את יישומי Microsoft 365 עבור enterprise ב-RDS מתוך מרכז הניהול של Microsoft 365, ***המשתמש בהגדרות ברירת המחדל של ההתקנה***, השתמש בשלבים הבאים.

> [!TIP]
> באפשרותך גם להוריד ולהפעיל את [מסייע התמיכה והשחזור של microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) כדי להתקין את יישומי microsoft 365 for enterprise במצב הפעלה משותפת של מחשב.
  
1. בדוק את מנוי Microsoft 365 שברשותך. [למד כיצד](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. במידת הצורך, עבור למנוי אחר של Microsoft 365. [למד כיצד](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. אם Office כבר מותקן בשרת RDS באמצעות מנויים אחרים של Microsoft 365, הסר את התקנתו. לדוגמה, על-ידי מעבר אל ' \> הסרת התקנה של תוכנית ' בלוח הבקרה. הסר התקנה באמצעות [מסייע התמיכה והשחזור של Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) אם אתה נתקל בבעיות.

4. בשרת RDS, היכנס למרכז הניהול של Microsoft 365 עם חשבון מנהל המערכת שלך [והתקן את יישומי microsoft 365 עבור הארגון](https://portal.office.com/OLS/MySoftware.aspx).

5. לאחר התקנת Office, ***אל תפתח או תיכנס*** ליישומי Office כלשהם.

6. בשרת RDS, אפשר הפעלת מחשב משותפת על-ידי עריכת הרישום על-ידי ביצוע השלבים הבאים:

1. לחץ באמצעות לחצן העכבר הימני על לחצן Windows בפינה הימנית התחתונה של המסך ובחר הרצה. בתיבה פתח, הקלד **regedit**ולאחר מכן בחר אישור.

2. בחר כן כאשר תתבקש לאפשר לעורך הרישום לבצע שינויים במכשיר שלך.

3. בעורך הרישום, הוסף ערך מחרוזת של **SharedComputerLicensing** עם הגדרה של 1 תחת HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.

7. בשרת RDS, ***היכנס כמשתמש קצה*** [וודא שהפעלת מחשב משותפת זמינה עבור יישומי Microsoft 365 for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

לקבלת פרטים נוספים על דרישות מוקדמות, הוראות הגדרה והנחיות לגבי התקנות מותאמות אישית באמצעות כלי הפריסה של Office, ראה [פריסת יישומי Microsoft 365 עבור enterprise באמצעות שירותי שולחן עבודה מרוחק](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
כדי לתקן שגיאות הקשורות להפעלת מחשב משותף, ראה [פתרון בעיות בהפעלת מחשב משותפת עבור יישומי Microsoft 365 עבור enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  