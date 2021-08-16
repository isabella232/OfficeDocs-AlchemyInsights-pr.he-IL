---
title: תיקון Microsoft 365 יישומים מצטערים, אנו נתקלים בהודעה של בעיות שרת זמניות
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
- "3420"
- "9001430"
ms.openlocfilehash: aa0d625856df1027146de5af57845224e3056d8c21d9ac4cefbd4a9c329f487c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54021597"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>תיקון Microsoft 365 "מצטערים, אנחנו נתקלים בבעיות שרת זמניות" הודעה

אם אתה מקבל הודעה זו, נסה את הפעולות הבאות:

1. בדוק את הגדרות חומת האש, תוכנת האנטי-וירוס וה- Proxy כדי לוודא שהם אינם חוסמים את הגישה לאינטרנט Microsoft 365 שלך. ראה [כתובות URL וטווחי כתובות IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. עבור אל  >  **התחל הפעלה** ולאחר מכן הקלד **services.msc**. ודא שהשירותים הבאים פועלים כולם:
    - התקנה אוטומטית של מכשירים מחוברים לרשת
    - שירות רשימת רשת
    - המודעות למיקום ברשת
    - Windows יומן אירועים

אם אחד מהשירותים הללו אינו פועל, נסה להפעיל אותו. אם יש לך בעיה בה הפעלת השירות, הפעל את הפקודה הבאה על-ידי פתיחת שורת פקודה עם הרשאות מלאות:

**sfc /scannow**

לאחר סיום פקודה זו, הפעל מחדש את המחשב.

לקבלת מידע מפורט, [ראה "מצטערים, אין לנו אפשרות להתחבר לחשבון שלך. נא נסה שוב מאוחר יותר" שגיאה בעת הפעלת](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).