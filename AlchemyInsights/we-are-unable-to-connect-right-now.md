---
title: בעיית הפעלה-אין באפשרותנו להתחבר כרגע
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
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725984"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>תיקון יישומי Microsoft 365 "אין באפשרותנו להתחבר כעת"

אם אתה מקבל הודעה זו, נסה את הפעולות הבאות:

1. בדוק את חומת האש, תוכנת האנטי-וירוס והגדרות ה-proxy כדי לוודא שהם אינם חוסמים את הגישה לאינטרנט ליישומי Microsoft 365. ראה [כתובות url וטווחי כתובות IP של Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. עבור אל **התחל**  >  **להפעיל**ולאחר מכן הקלד **services. msc**. ודא שהשירותים הבאים פועלים כולם:
    - התקנה אוטומטית של התקנים מחוברים לרשת
    - שירות רשימת הרשתות
    - מודעות למיקום ברשת
    - יומן האירועים של Windows

אם אחד מהשירותים האלה אינו פועל, נסה להפעיל אותו. אם אתה נתקל בבעיה בהפעלת השירות, הפעלת הפקודה הבאה על-ידי פתיחת שורת פקודה עם הרשאות מלאות:

**sfc/scannow**

לאחר שפקודה זו מסתיימת, הפעל מחדש את המחשב.

לקבלת מידע מפורט, ראה ["מצטערים, אין לנו אפשרות להתחבר לחשבון שלך. נסה שוב מאוחר יותר את השגיאה כאשר אתה מפעיל את Office מ-Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).