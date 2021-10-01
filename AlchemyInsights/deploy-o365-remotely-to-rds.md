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
ms.openlocfilehash: 9d928a3bf58dedc3aaf231c8a051f87b0bbdf438
ms.sourcegitcommit: 391052026a6ce7646926d233d0fd9ba135088f79
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/01/2021
ms.locfileid: "60041007"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>פריסת יישומי Microsoft 365 לארגונים לשימוש משותף ב- RDS , Terminal Server או VDI

כדי לפרוס יישומי Microsoft 365 שירותי שולחן עבודה מרוחק (RDS), בעבר שירותי מסוף, עליך:

- השתמש בתיקון קל כדי להפוך את TLS 1.2 לזמין כברירת מחדל אם אתה משתמש בגירסה קודמת של Windows (לדוגמה, Windows 7 SP1, Windows Server 2008 R2). לקבלת תיקון קל ומידע נוסף, ראה עדכון כדי להפוך [את TLS 1.1 ו- TLS 1.2](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy)לזמינים כפרוטוקולים מאובטחים המוגדרים כברירת מחדל ב- WinHTTP ב- Windows. 
- יש לך תוכנית הכוללת את יישומי Microsoft 365 לארגונים (בעבר Office 365 Plus). לדוגמה, Office 365 E3 או Microsoft 365 E5, או כל תוכנית הכוללת את גירסת שולחן העבודה של Project או Visio, כגון Project תוכנית 3 או Visio תוכנית 2, או תוכנית Microsoft 365 Business Premium, הכוללת גם יישומי Microsoft 365 לעסקים.
- הפוך הפעלת מחשב משותפת לזמינה. לקבלת מידע נוסף, ראה [מבט כולל על הפעלת מחשב משותפת עבור יישומי Microsoft 365](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation).

**הערה:** כדי להתקין יישומי Microsoft 365 במצב הפעלת מחשב משותף, הורד והפעל את [Microsoft מסייע התמיכה והשחזור.](https://docs.microsoft.com/alchemyinsights/deploy-o365-remotely-to-rds) לקבלת פרטים על דרישות מוקדמות, הוראות הגדרה והדרכה להתאמה אישית של התקנות באמצעות כלי הפריסה של Office, [ראה פריסת יישומי Microsoft 365 באמצעות שירותי שולחן עבודה מרוחק](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services).

כדי לתקן שגיאות הקשורות להפעלת מחשב משותף, ראה:

- [פתרון בעיות בהפעלת מחשב משותפת עבור יישומי Microsoft 365](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [איפוס יישומי Microsoft 365 Apps עבור מצב enterprise activation state](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

אם ברצונך להתקין את יישומי Microsoft 365 ב- RDS מתוך מרכז הניהול של Microsoft 365, המשתמש בהגדרות ההתקנה המהוות ברירת מחדל, בצע את הפעולות הבאות:

1. בדוק איזו תוכנית Microsoft 365 יש לך. לקבלת מידע נוסף, [ראה איזה מנוי יש לי?](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).

1. במקרה הצורך, עבור לתוכנית Microsoft 365 אחרת. לקבלת מידע נוסף, [ראה שדרוג לתוכנית אחרת](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan).

1. אם יישומי Microsoft 365 כבר מותקן בשרת RDS באמצעות תוכניות לא תואמות אחרות, הסר את התקנתו על-ידי עבור אל **לוח הבקרה** הסר  >  **התקנת תוכנית.** אם אתה נכנס לבעיות, הסר את ההתקנה על-ידי [הורדת Microsoft מסייע התמיכה והשחזור](https://aka.ms/SARA-OfficeUninstall-Alchemy).

1. בשרת RDS, היכנס אל מרכז הניהול של Microsoft 365 עם חשבון מנהל המערכת שלך [והתקן Office.](https://portal.office.com/OLS/MySoftware.aspx)

   לאחר Office, אל תפתח או היכנס ליישומים Office אחרים.

1. בשרת RDS, הפוך הפעלת מחשב משותף לזמינה על-ידי עריכת הרישום:

   1. לחץ באמצעות לחצן Windows לחצן העכבר הימני בפינה הימנית התחתונה של המסך ובחר **הפעל**. בתיבה פתח, הקלד **regedit**, ולאחר מכן בחר **אישור**.

   1. כאשר תתבקש לאפשר לעורך הרישום לבצע שינויים במכשיר שלך, בחר **כן**.

   1. בעורך הרישום, תחת HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration, הוסף ערך מחרוזת **של SharedComputerlicensing** עם הגדרה של **1** .

1. בשרת RDS, היכנס כמשתמש קצה וודא שהפעלת מחשב משותפת זמינה עבור יישומי Microsoft 365. 

   לקבלת פרטים, [ראה אימות הפעלת מחשב משותפת זו זמינה עבור יישומי Microsoft 365.](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps)