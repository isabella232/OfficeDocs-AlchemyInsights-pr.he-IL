---
title: פריסת יישומי Microsoft 365 עבור enterprise לשימוש משותף ב-RDS, Terminal Server או VDI
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
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200674"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>פריסת יישומי Microsoft 365 עבור enterprise לשימוש משותף ב-RDS, Terminal Server או VDI

כדי לפרוס את יישומי Microsoft 365 עבור enterprise באמצעות שירותי שולחן עבודה מרוחק (RDS), שנקראו בעבר ' שירותי מסוף ':

- דרושה לך תוכנית Microsoft 365 For Business או תוכנית של Office 365 הכוללת אפליקציות של Microsoft 365 לארגונים, כגון Office 365 Enterprise E3 או Enterprise E5.
   > [!NOTE]
   > התוכניות הסטנדרטיות של microsoft 365 לעסקים ו-Microsoft 365 אינן כוללות אפליקציות של Microsoft 365 עבור הארגון.
- עליך להפוך [הפעלת מחשב משותפת](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)לזמינה.

> [!NOTE]
> באפשרותך גם להוריד ולהפעיל את [מסייע התמיכה והשחזור של microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) כדי להתקין את יישומי microsoft 365 for enterprise במצב הפעלה משותפת של מחשב.

לקבלת מידע נוסף אודות דרישות מוקדמות, הוראות הגדרה והנחיות לגבי התקנות מותאמות אישית באמצעות כלי הפריסה של Office, ראה [פריסת יישומי Microsoft 365 עבור enterprise באמצעות שירותי שולחן עבודה מרוחק](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

כדי לתקן שגיאות הקשורות להפעלת מחשב משותפת:

- ראה [פתרון בעיות בהפעלת מחשב משותף עבור יישומי Microsoft 365 עבור enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- ראה [איפוס יישומי Microsoft 365 עבור מצב הפעלה ארגונית](https://go.microsoft.com/fwlink/?linkid=2109218).

אם ברצונך להתקין את יישומי Microsoft 365 עבור enterprise ב-RDS מתוך מרכז הניהול של Microsoft 365, ***המשתמש בהגדרות ההתקנה המשמשות כברירת מחדל***, השתמש בשלבים הבאים:

1. בדוק איזה מנוי יש לך. [למד כיצד לעשות זאת](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. במידת הצורך, עבור למנוי אחר. [למד כיצד לעשות זאת](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. אם Office כבר מותקן בשרת RDS באמצעות מנויים אחרים של Microsoft, הסר את התקנתו. לדוגמה, על-ידי מעבר אל **'**  >  **הסרת התקנה של תוכנית ' בלוח הבקרה**. הסר התקנה באמצעות [מסייע התמיכה והשחזור של Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) אם אתה נתקל בבעיות.
4. בשרת RDS, היכנס למרכז הניהול של Microsoft 365 עם חשבון מנהל המערכת שלך [והתקן את יישומי microsoft 365 עבור הארגון](https://portal.office.com/OLS/MySoftware.aspx).
5. לאחר התקנת Office, ***אל תפתח או תיכנס*** ליישומי Office כלשהם.
6. בשרת RDS, אפשר הפעלת מחשב משותפת על-ידי עריכת הרישום על-ידי ביצוע השלבים הבאים:
   1. לחץ באמצעות לחצן העכבר הימני על לחצן Windows בפינה הימנית התחתונה של המסך ובחר **הרצה**. בתיבה פתח, הקלד **regedit**, ולאחר מכן בחר **אישור**.
   2. בחר **כן** כאשר תתבקש לאפשר לעורך הרישום לבצע שינויים במכשיר שלך.
   3. בעורך הרישום, הוסף ערך מחרוזת של **SharedComputerLicensing** עם הגדרה של 1 תחת HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. בשרת RDS, ***היכנס כמשתמש קצה*** [וודא שהפעלת מחשב משותפת זמינה עבור יישומי Microsoft 365 for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).
