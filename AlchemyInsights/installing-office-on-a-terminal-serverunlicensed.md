---
title: התקנת office בשרת מסופים - ללא רשיון
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 73d5128b55cae7712c48be9e2d05e558c3ba2e5c
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29472413"
---
# <a name="installing-office-on-a-terminal-server"></a>התקנת Office בשרת מסופים

לפריסת Office 365 ProPlus בשרת Windows באמצעות שירותי שולחן עבודה מרוחק (RDS), לשעבר בשם שירותי מסופים:
  
- דרושה לך תוכנית Office 365 הכוללת Office 365 ProPlus, כגון Office 365 ארגון E3 או ארגון E5. תוכניות Office 365 עסקיים ו- Office 365 עסקיים איכותיים אינם כוללים ProPlus של Office 365.
    
- עליך לאפשר [הפעלה במחשב משותף](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).
    
אם ברצונך להתקין את Office 365 ProPlus RDS מתוך הפורטל Office 365, * * *המשתמשת הגדרות ברירת המחדל של ההתקנה* * *, בצע את הפעולות הבאות: 
  
1. בדוק איזו תוכנית Office 365 יש לך. [ללמוד כיצד](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. אם מתכננים הצורך, מתג Office 365 שונים. [ללמוד כיצד](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. אם כבר התקנת Office בשרת RDS באמצעות כל תוכניות אחרות של Office 365, הסר אותו. לדוגמה, על-ידי מעבר אל לוח הבקרה \> להסיר התקנה של תוכנית. הסרת התקנה באמצעות [התמיכה של Microsoft ומסייע שחזור](https://aka.ms/SARA-OfficeUninstall-Alchemy) אם אתה מפעיל לתוך בעיות. 
    
4. בשרת RDS, היכנס אל פורטל Office 365 עם שלך חשבון מנהל המערכת ולהתקין את [Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
    
5. לאחר התקנת Office, * * *אין לפתוח או להיכנס* * * כל יישומי Office. 
    
6. בשרת RDS, לאפשר הפעלה במחשב משותף על-ידי עריכת הרישום על-ידי ביצוע השלבים הבאים:
    
1. לחץ לחיצה ימנית על לחצן Windows בפינה הימנית התחתונה של המסך, ובחר באפשרות הפעלה. בתיבה פתח את, הקלד **regedit**ולאחר מכן לחץ על אישור. 
    
2. בחר באפשרות כן כאשר תתבקש לאפשר בעורך הרישום כדי לבצע שינויים למכשיר שלך.
    
3. בעורך הרישום, הוסף ערך מחרוזת של **SharedComputerLicensing** עם הגדרה של 1 תחת HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration. 
    
7. בשרת RDS, * * *היכנס בתור משתמש קצה* * *, [וודא כי הפעלת מחשב משותף זמין עבור Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).
    
לקבלת פרטים נוספים על תנאים מוקדמים, הוראות ההתקנה והדרכה לגבי התקנות מותאמות אישית על-ידי שימוש בכלי הפריסה של Office, נא ראה [פריסת Office 365 ProPlus באמצעות שירותי שולחן עבודה מרוחק](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
כדי לתקן שגיאות הקשורות להפעלת מחשב משותף, נא ראה [פתרון בעיות עם הפעלת מחשב משותף עבור Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  

