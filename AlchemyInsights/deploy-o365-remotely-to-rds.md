---
title: פריסת Office 365 ProPlus עבור שימוש משותף ב-RDS, שרת מסופים או VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959461"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>פריסת Office 365 ProPlus עבור שימוש משותף ב-RDS, שרת מסופים או VDI

כדי לפרוס את Office 365 ProPlus באמצעות שירותי שולחן עבודה מרוחק (RDS), שנקרא בעבר שירותי מסוף:
- עליך להיות בעל 365 של Microsoft עבור תוכנית עסקית או תוכנית Office 365 הכוללת את Office 365 ProPlus, כגון Office 365 E3 או באמצעות הארגון E5.
   > [!NOTE] 
   > התוכניות של Office 365 Business ו-Office 365 Business Premium אינן כוללות את Office 365 ProPlus.
- עליך להפוך [הפעלת מחשב משותפת](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)לזמינה.

> [!NOTE]
> באפשרותך גם להוריד ולהפעיל את [מסייע התמיכה והשחזור של Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) כדי להתקין את Office 365 proplus במצב משותף של הפעלת מחשב.

לקבלת מידע נוסף אודות דרישות מוקדמות, הוראות התקנה והנחיות בנוגע להתקנות מותאמות אישית באמצעות כלי הפריסה של Office, ראה [פריסת office 365 ProPlus באמצעות שירותי שולחן עבודה מרוחק](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

כדי לתקן שגיאות הקשורות להפעלת מחשב משותף:
- ראה [פתרון בעיות בהפעלת מחשב משותף עבור Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- ראה [איפוס מצב ההפעלה של Office 365 ProPlus](https://go.microsoft.com/fwlink/?linkid=2109218).

אם ברצונך להתקין את Office 365 ProPlus ב-RDS ממרכז הניהול של Microsoft 365, ***המשתמש בהגדרות ברירת המחדל של ההתקנה***, השתמש בשלבים הבאים:

1.  בדוק מה תוכנית Office 365 יש לך. [למד כיצד לעשות זאת](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.  במקרה הצורך, עבור לתוכנית אחרת של Office 365. [למד כיצד לעשות זאת](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.  אם Office כבר מותקן בשרת RDS באמצעות כל תוכנית אחרת של Office 365, הסר את התקנתה. לדוגמה, על-ידי הולך **ללוח** > **הבקרה הסר תוכנית**. הסר [התקנה באמצעות מסייע התמיכה והשחזור של Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) אם אתה נתקל בבעיות.
4.  בשרת RDS, היכנס למרכז הניהול של Microsoft 365 עם חשבון מנהל המערכת שלך [והתקן את Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
5.  לאחר התקנת Office, ***אל תפתח או תיכנס*** ליישומי office כלשהם.
6.  בשרת RDS, הפעל הפעלה משותפת של המחשב על-ידי עריכת הרישום על-ידי ביצוע השלבים הבאים:
   1. לחץ לחיצה ימנית על לחצן Windows בפינה השמאלית התחתונה של המסך ובחר באפשרות **הפעלה**. בתיבה פתח את, הקלד **regedit**ולאחר מכן בחר **באפשרות אישור**.
   2. בחר **כן** כאשר תתבקש לאפשר לעורך הרישום לבצע שינויים במכשיר.
   3. בעורך הרישום, הוסף ערך מחרוזת של **רישוי שיתופיות** עם הגדרה של 1 תחת HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.
   4. בשרת RDS, ***היכנס כמשתמש קצה*** [וודא שהפעלת מחשב משותף זמינה עבור Office 365 proplus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

