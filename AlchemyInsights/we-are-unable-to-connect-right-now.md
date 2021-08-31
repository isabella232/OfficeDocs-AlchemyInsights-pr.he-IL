---
title: בעיית הפעלה - אין באפשרותנו להתחבר כעת
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 0ab831696736352bf9de84f43c96bb8f7238d8eb
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744596"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>תיקון ההודעה Microsoft 365 "אין באפשרותנו להתחבר כעת"

הערה: אם אתה משתמש בגירסה קודמת של Windows (לדוגמה, Windows 7 SP1, Windows Server 2008 R2), השתמש בתיקון הקלה כדי [להפוך](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) את TLS 1.2 לזמין כברירת מחדל. לקבלת מידע נוסף, ראה [עדכון כדי להפוך את TLS 1.1 ו- TLS 1.2 לזמינים](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)כפרוטוקולים מאובטחים המהווים ברירת מחדל ב- WinHTTP ב- Windows.

אם אתה מקבל הודעה זו, נסה את הפעולות הבאות:

1. בדוק את הגדרות חומת האש, תוכנת האנטי-וירוס וה- Proxy כדי לוודא שהם אינם חוסמים גישה לאינטרנט Microsoft 365 יישומים. ראה [כתובות URL של Microsoft וטווחי כתובות IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. עבור אל  >  **התחל הפעלה** ולאחר מכן הקלד **services.msc**. ודא שהשירותים הבאים פועלים כולם:
    - התקנה אוטומטית של מכשירים מחוברים לרשת
    - שירות רשימת רשת
    - המודעות למיקום ברשת
    - Windows יומן אירועים

אם אחד מהשירותים הללו אינו פועל, נסה להפעיל אותו. אם יש לך בעיה בה הפעלת השירות, הפעל את הפקודה הבאה על-ידי פתיחת שורת פקודה עם הרשאות מלאות:

**sfc /scannow**

לאחר סיום פקודה זו, הפעל מחדש את המחשב.

לקבלת מידע מפורט, [ראה "מצטערים, אין לנו אפשרות להתחבר לחשבון שלך. נסה שוב מאוחר יותר" שגיאה בעת הפעלת Office מ- Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).