---
title: בעיות בכניסה לאפליקציות Microsoft 365 שלך
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
- "9000571"
- "2559"
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986892"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>הודעת תיקון Microsoft 365 "מודול הפלטפורמה המהימנה של המחשב שלך אינו פועל כראוי"

כדי לתקן שגיאה זו, נסה את השלבים הבאים:

- התקן את העדכונים האחרונים [עבור Windows ו-](https://support.microsoft.com/help/4027667/windows-10-update) [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [נקה Office אישורי](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) Windows מנהל האישורים.<br/>
    **הערה:** נתיבי הרישום עבור Office 2016 השתנו ל- 16.0. (לדוגמה: \Software\Microsoft\Office\16.0\Common\Identity\)
- נסה את [תהליך שחזור המשתמשים כדי](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) לתקן כשלים במודול פלטפורמה מהימנה (TPM).
- הגדר את EnableADAL = 0 באמצעות השלבים הבאים:  
    1. לחץ באמצעות לחצן העכבר הימני Windows התחל, בחר **הפעל**, הקלד **regedit** ולאחר מכן בחר **אישור**.
    2. בחר **כן** כדי לאפשר לעורך הרישום לבצע שינויים במכשיר שלך.
    3. בעורך הרישום, הוסף ערך DWORD של **EnableADAL** עם הגדרה של **0 תחת** HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

לקבלת מידע נוסף, ראה בעיות חיבור בהתחברות לאחר עדכון [ל- Office גירסת Build מס' 16.0.7967 ב- Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)