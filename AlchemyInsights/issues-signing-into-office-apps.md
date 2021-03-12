---
title: בעיות בכניסה ליישומי Microsoft 365
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
- "9000571"
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709107"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>תיקון יישומי Microsoft 365 "מודול הפלטפורמה המהימנה של המחשב שלך אינו פועל כהלכה"

כדי לתקן שגיאה זו, נסה את השלבים הבאים:

- התקן את העדכונים האחרונים עבור [Windows](https://support.microsoft.com/help/4027667/windows-10-update) ו- [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [נקה את אישורי Office](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) באמצעות מנהל האישורים של Windows.<br/>
    **הערה:** נתיבי הרישום של Office 2016 השתנו ל-16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- נסה את [תהליך שחזור המשתמש](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) כדי לתקן כשלים של מודול פלטפורמה מהימנה (TPM).
- הגדר את EnableADAL = 0 באמצעות השלבים הבאים:  
    1. לחץ באמצעות לחצן העכבר הימני על לחצן התחל של Windows, בחר **הפעל**, הקלד **regedit** ולאחר מכן בחר **אישור**.
    2. בחר **כן** כדי לאפשר לעורך הרישום לבצע שינויים במכשיר שלך.
    3. בעורך הרישום, הוסף ערך DWORD של **EnableADAL** עם הגדרה של **0** תחת HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

לקבלת מידע נוסף, ראה [בעיות חיבור בכניסה לאחר עדכון ל-Office 2016 build 16.0.7967 ב-Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).