---
title: בעיות בכניסה לאפליקציות של Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579866"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>תיקון יישומי Microsoft 365 "מודול הפלטפורמה המהימנה של המחשב אינו פועל כראוי" הודעה

כדי לתקן שגיאה זו, נסה את השלבים הבאים:

- התקן את העדכונים האחרונים עבור [Windows](https://support.microsoft.com/help/4027667/windows-10-update) ו- [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [נקה אישורי Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) באמצעות מנהל האישורים של Windows.<br/>
    **הערה:** נתיבי הרישום עבור Office 2016 השתנו ל-16.0. (לשעבר: \Software\Microsoft\Office\16.0\Common\Identity\)
- נסה את [תהליך השחזור של המשתמש](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) כדי לתקן כשלים של מודול פלטפורמה מהימנה (TPM).
- הגדר את האפשרות Enabto Al = 0 באמצעות השלבים הבאים:  
    1. לחץ לחיצה ימנית על לחצן התחל של Windows, בחר באפשרות **הפעלה**, הקלד **regedit**ולאחר מכן בחר **באפשרות אישור**.
    2. בחר **כן** כדי לאפשר לעורך הרישום לבצע שינויים במכשיר.
    3. בעורך הרישום, הוסף ערך DWORD של **אפשור להפניה** עם הגדרה של **0** תחת HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.

לקבלת מידע נוסף, ראה [בעיות חיבור בכניסה לאחר עדכון ל-Office 2016 build 16.0.7967 ב-Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).