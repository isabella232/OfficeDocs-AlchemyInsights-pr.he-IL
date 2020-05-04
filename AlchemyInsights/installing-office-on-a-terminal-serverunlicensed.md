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
ms.openlocfilehash: 6e952513679c9ac66f8de2b43d6d243cf17ff789
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010615"
---
# <a name="installing-office-on-a-terminal-server"></a>התקנת Office בשרת מסופים

לפריסת יישומי Microsoft 365 עבור ארגון בשרת Windows באמצעות שירותי שולחן עבודה מרוחק (RDS), ששמו בעבר שירותי מסופים:
  
- עליך לכלול מנוי של Microsoft 365 הכולל את Microsoft 365 Apps עבור ארגון, כגון Office 365 Enterprise E3 או Enterprise E5. מיקרוסופט 365 Apps עבור עסקים ו-Microsoft 365 Apps עבור עסקים תוכניות פרימיום אינם כוללים Microsoft 365 Apps עבור הארגון.

- עליך להפוך [הפעלת מחשב משותפת](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)לזמינה.

אם ברצונך להתקין את Microsoft 365 Apps עבור ארגון ב-RDS ממרכז הניהול של Microsoft 365, ***המשתמש בהגדרות ברירת המחדל של ההתקנה***, השתמש בשלבים הבאים.

> [!TIP]
> באפשרותך גם להוריד ולהפעיל את [מסייע התמיכה והשחזור של microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) כדי להתקין את Microsoft 365 Apps עבור ארגון במצב הפעלה משותף של המחשב.
  
1. בדוק מה מנוי 365 של Microsoft שקיבלת. [למד כיצד](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. במקרה הצורך, עבור למנוי אחר של Microsoft 365. [למד כיצד](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. אם Office כבר מותקן בשרת ה-RDS באמצעות כל מנוי אחר של Microsoft 365, הסר את התקנתה. לדוגמה, על-ידי הדרך \> ללוח הבקרה הסר תוכנית. הסר [התקנה באמצעות מסייע התמיכה והשחזור של Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) אם אתה נתקל בבעיות.

4. בשרת RDS, היכנס למרכז הניהול של Microsoft 365 עם חשבון מנהל המערכת שלך [והתקן את microsoft 365 Apps עבור הארגון](https://portal.office.com/OLS/MySoftware.aspx).

5. לאחר התקנת Office, ***אל תפתח או תיכנס*** ליישומי office כלשהם.

6. בשרת RDS, הפעל הפעלה משותפת של המחשב על-ידי עריכת הרישום על-ידי ביצוע השלבים הבאים:

1. לחץ לחיצה ימנית על לחצן Windows בפינה השמאלית התחתונה של המסך ובחר באפשרות הפעלה. בתיבה פתח את, הקלד **regedit**ולאחר מכן בחר באישור.

2. בחר כן כאשר תתבקש לאפשר לעורך הרישום לבצע שינויים במכשיר.

3. בעורך הרישום, הוסף ערך מחרוזת של **רישוי שיתופיות** עם הגדרה של 1 תחת HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.

7. בשרת RDS, ***היכנס כמשתמש קצה*** [וודא שהפעלת מחשב משותף מאופשרת עבור יישומי Microsoft 365 עבור הארגון](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

לקבלת פרטים נוספים על דרישות מוקדמות, הוראות התקנה והדרכה בהתקנות מותאמות אישית באמצעות כלי הפריסה של Office, עיין [בפריסת Microsoft 365 Apps לארגון באמצעות שירותי שולחן עבודה מרוחק](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
כדי לתקן שגיאות הקשורות להפעלת מחשב משותף, ראה [פתרון בעיות בהפעלה משותפת של מחשב עבור Microsoft 365 Apps עבור הארגון](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  