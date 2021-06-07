---
title: לא ניתן להפעיל את Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798681"
---
# <a name="unable-to-activate-office"></a>לא ניתן להפעיל את Office

**הערה**: אם אתה משתמש בגירסה קודמת של Windows (לדוגמה, Windows 7), ודא ש- TLS 1.2 זמין כברירת המחדל. לקבלת מידע נוסף, ראה [עדכון כדי להפוך את TLS 1.1 ו- TLS 1.2 לזמינים](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)כפרוטוקולים מאובטחים המהווים ברירת מחדל ב- WinHTTP ב- Windows.

- בדוק אם מצב המינוי שלך פג.
- ודא שיש לך מנוי המאפשר רשיונות לקוח, כגון Office 365 Business או Business Premium, ו[ודא שלמשתמש הוקצה רשיון](/microsoft-365/admin/manage/assign-licenses-to-users).
- ודא שהמשתמש נכנס ל- Office באמצעות אותו החשבון שהוקצה לו רשיון.
- בדוק את [דף תקינות השירות של Office 365](/office365/enterprise/view-service-health) כדי לבדוק אם יש בעיות ידועות בשירות.
- בדוק את חומת האש, תוכנת האנטי-וירוס והגדרות שרת ה- proxy כדי לוודא שהוא אינו חוסם את הגישה של יישומי Microsoft 365 לאינטרנט. עיין ב[כתובות URL וטווחי כתובות IP של Office 365](/office365/enterprise/urls-and-ip-address-ranges "כתובות URL וטווחי כתובות IP של Office 365").

**עצה** במחשבי Windows, אנו יכולים לאבחן ולפתור עבורך באופן אוטומטי כמה בעיות כניסה נפוצות של Office. הורד והפעל את  **[מסייע התמיכה והשחזור של Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** כדי להשתמש בכלי האוטומטי שלנו.

השתמש בפעולות פתרון הבעיות הבאות:

- פתח יישום של Office ו[צא](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) מחשבונות משתמשים קיימים. [הסרה](/microsoft-365/admin/manage/remove-licenses-from-users) ו[הקצה מחדש](/microsoft-365/admin/manage/assign-licenses-to-users) רישיון Office ולאחר מכן [היכנס ל- Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) באמצעות חשבון המשתמש המושפע.
- הפעל את ['פותר בעיות ההפעלה'](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [איפוס מצב ההפעלה של Office](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "איפוס מצב ההפעלה של Office")
- [בצע תיקון מקוון של Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

לפתרונות נוספים, ראה:  

- [שגיאות מסוג "מוצר ללא רישיון" ושגיאות הפעלה ב- Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [השגיאה "מצטערים, אין לנו אפשרות להתחבר לחשבון שלך. נסה שוב במועד מאוחר יותר"בעת הפעלת Office](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)