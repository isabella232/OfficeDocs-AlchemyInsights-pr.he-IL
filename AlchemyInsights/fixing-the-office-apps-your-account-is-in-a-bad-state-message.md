---
title: תיקון יישומי Office החשבון שלך נמצא בהודעת מצב לא טובה
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969495"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>תיקון היישומים של Office "החשבון שלך במצב רע" שגיאה

כדי לתקן שגיאה זו, נסה את האפשרויות הבאות במחשב המושפע:

- פתח יישום Office, בחר את > **החתימה של****חשבון** **הקובץ** > מכל החשבונות. היכנס שוב באמצעות חשבון משתמש עם רשיון חוקי. לקבלת מידע מפורט, ראה [תיקי לקוחות ב-Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [נקה אישורי Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) באמצעות מנהל האישורים של Windows.<br>
  **הערה:** נתיבי הרישום עבור Office 2016 השתנו ל-16.0. לדוגמה, \Software\Microsoft\Office\16.0\Common\Identity\
- במחשב המושפע, הגדר את האפשרות Enabהפניות אל = 0 באמצעות השלבים הבאים:  
     1. לחץ לחיצה ימנית על לחצן Windows ובחר באפשרות **הפעלה**. בתיבה **פתח את** , הקלד **regedit**ולאחר מכן בחר **באפשרות אישור**.
     2. בחר **כן** כאשר תתבקש לאפשר לעורך הרישום לבצע שינויים במכשיר.
    3. בעורך הרישום, הוסף ערך DWORD של Enabמסוף עם הגדרה של 0 תחת HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.
- אם השגיאה מתרחשת בעת התחברות ל-Office 365 באמצעות Office 2013, [הפעל אימות מודרני](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) עבור לקוח office.

לקבלת מידע נוסף, ראה [כיצד לפתור בעיות ביישומים שאינם של הדפדפן שאינם יכולים להיכנס ל-Office 365, תכלת או Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

