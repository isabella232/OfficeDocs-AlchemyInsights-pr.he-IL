---
title: תיקון יישומי Office מצטערים, יש לנו הודעה על בעיות שרת זמניות
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764118"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>תיקון יישומי Office "מצטערים, יש לנו בעיות שרת זמניות" הודעה

אם תקבל הודעה זו, נסה את הפעולות הבאות:

1. בדוק את חומת האש, תוכנת האנטי-וירוס והגדרות ה-proxy כדי לוודא שהן אינן חוסמות גישה לאינטרנט ליישומי Office. ראה [כתובות url וטווחי כתובות IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. עבור **להתחלת** > **הפעלה**ולאחר מכן הקלד **services. msc**. ודא שהשירותים הבאים פועלים:
    - התקנה אוטומטית של התקני רשת מחוברים
    - שירות רשימת הרשתות
    - מיקום רשת מודעות
    - יומן האירועים של Windows

אם אחד מהשירותים הללו אינו פועל, נסה להפעיל אותו. אם יש לך בעיה בהפעלת השירות, הפעל את הפקודה הבאה על-ידי פתיחת שורת פקודה עם הרשאות מוגברות:

**sfc/scannow**

לאחר סיום פקודה זו, הפעל מחדש את המחשב.

למידע מפורט, ראה [מצטערים, איננו יכולים להתחבר לחשבונך. נא נסה שוב מאוחר יותר את השגיאה כאשר אתה מפעיל](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).