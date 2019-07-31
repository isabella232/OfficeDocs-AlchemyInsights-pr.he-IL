---
title: בעיות הכניסה אל יישומי Office
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
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938232"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>תיקון ההודעה "מודול פלטפורמה מהימנים של המחשב שלך אינו פועל כראוי" יישומי Office

כדי לתקן שגיאה זו, נסה לבצע את הפעולות הבאות:

- התקן את העדכונים האחרונים עבור [Windows](https://support.microsoft.com/help/4027667/windows-10-update) ו- [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [אישורי Office ניקוי](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) באמצעות מנהל האישורים של Windows.<br/>
    **הערה:** נתיבי רישום עבור Office 2016 השתנו כדי 16.0. (לדוגמה: \Software\Microsoft\Office\16.0\Common\Identity\)
- נסה את [תהליך השחזור של המשתמש](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) כדי לתקן כשלים Trusted Platform Module (TPM).
- הגדר את EnableADAL = 0 באמצעות השלבים הבאים:  
    1. באמצעות לחצן העכבר הימני על לחצן התחל של Windows, בחר באפשרות **הפעל**, הקלד **regedit**ולאחר מכן לחץ על **אישור**.
    2. בחר **כן** כדי לאפשר בעורך הרישום כדי לבצע שינויים למכשיר שלך.
    3. בעורך הרישום, הוסף ערך DWORD של **EnableADAL** עם הגדרה של **0** תחת HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

לקבלת מידע נוסף, ראה [חיבור בעיות בהכניסה לאחר העדכון ל- Office 2016 build 16.0.7967 על Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).