---
title: תיקון יישומי Microsoft 365 מצטערים, אנו נתקלים בהודעת בעיות שרת זמניות
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758246"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>תיקון יישומי Microsoft 365 "מצטערים, אנו נתקלים בבעיות שרת זמני"

אם אתה מקבל הודעה זו, נסה את הפעולות הבאות:

1. בדוק את חומת האש, תוכנת האנטי-וירוס והגדרות ה-proxy כדי לוודא שהם אינם חוסמים את הגישה לאינטרנט ליישומי Microsoft 365. ראה [כתובות url וטווחי כתובות IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. עבור אל **התחל**  >  **להפעיל**ולאחר מכן הקלד **services. msc**. ודא שהשירותים הבאים פועלים כולם:
    - התקנה אוטומטית של התקנים מחוברים לרשת
    - שירות רשימת הרשתות
    - מודעות למיקום ברשת
    - יומן האירועים של Windows

אם אחד מהשירותים האלה אינו פועל, נסה להפעיל אותו. אם אתה נתקל בבעיה בהפעלת השירות, הפעלת הפקודה הבאה על-ידי פתיחת שורת פקודה עם הרשאות מלאות:

**sfc/scannow**

לאחר שפקודה זו מסתיימת, הפעל מחדש את המחשב.

לקבלת מידע מפורט, ראה ["מצטערים, אין לנו אפשרות להתחבר לחשבון שלך. נסה שוב במועד מאוחר יותר את השגיאה בעת ההפעלה](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).