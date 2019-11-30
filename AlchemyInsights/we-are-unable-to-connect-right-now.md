---
title: סוגיית ההפעלה-אין באפשרותנו להתחבר כרגע
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628243"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>תיקון האפליקציות של Office "אנחנו לא יכולים להתחבר כרגע" הודעה

אם תקבל הודעה זו, נסה את הפעולות הבאות:

1. בדוק את חומת האש, תוכנת האנטי-וירוס והגדרות ה-proxy כדי לוודא שהן אינן חוסמות גישה לאינטרנט ליישומי Office. ראה [כתובות Url של Office 365 וטווחי כתובות IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. עבור **להתחלת** > **הפעלה**ולאחר מכן הקלד **services. msc**. ודא שהשירותים הבאים פועלים:
    - התקנה אוטומטית של התקני רשת מחוברים
    - שירות רשימת הרשתות
    - מיקום רשת מודעות
    - יומן האירועים של Windows

אם אחד מהשירותים הללו אינו פועל, נסה להפעיל אותו. אם יש לך בעיה בהפעלת השירות, הפעל את הפקודה הבאה על-ידי פתיחת שורת פקודה עם הרשאות מוגברות:

**sfc/scannow**

לאחר סיום פקודה זו, הפעל מחדש את המחשב.

למידע מפורט, ראה [מצטערים, איננו יכולים להתחבר לחשבונך. נא נסה שוב מאוחר יותר את השגיאה בעת הפעלת Office מ-Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).