---
title: לקוח Teams קורס?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826272"
---
# <a name="teams-client-crashing"></a>לקוח Teams קורס?

אם לקוח Teams שלך קורס, נסה את הפעולות הבאות:

- אם אתה משתמש ביישום שולחן העבודה של Teams, [ודא שהיישום מעודכן במלואו](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- ודא שכל כתובות ה- [URL וטווחי הכתובות של Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) נגישות.

- היכנס באמצעות חשבון מנהל הדייר שלך ובדוק את לוח [המחוונים](https://docs.microsoft.com/office365/enterprise/view-service-health) של תקינות השירות כדי לוודא שלא קיימים בעיות של מחסור או שפלת שירות.

- הסרת התקנה והתקנה מחדש של יישום Teams (קישור)
    - עבור אל התיקיה %appdata%\Microsoft\teams\ במחשב שלך ומחק את כל הקבצים במדריך כתובות זה.
    - [הורד והתקן את היישום Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), ואם הדבר אפשרי, התקן את Teams כמנהל מערכת (לחץ באמצעות לחצן העכבר הימני על המתקין Teams ובחר "הפעל כמנהל" אם זמין).

אם לקוח Teams שלך עדיין קורס, תוכל לשחזר את הבעיה? אם כן:

1. השתמש במקליט השלבים כדי ללכוד את השלבים שלך.
    - סגור את ALL יישומים לא נחוצים או סודיים.
    - הפעל את מקליט השלבים ושכפול הבעיה בעת כניסה באמצעות חשבון המשתמש המושפע.
    - [אסוף את יומני הרישום של הצוותים שלכודים את שלבי השכפול המוקלטים.](https://docs.microsoft.com/microsoftteams/log-files) **הערה:** הקפד ללכוד את כתובת הכניסה של המשתמש מושפע.
    - אסוף את פרטי ה- dump ו/או הדלי של תקלות (Windows). הפעל את Windows Powershell במחשב שבו מתרחשת קריסה ולהפעיל את הפקודות הבאות:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. צרף את הקובץ למקרה התמיכה שלך.
