---
title: לקוח Teams קורס?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354053"
---
# <a name="teams-client-crashing"></a>לקוח Teams קורס?

אם לקוח Teams שלך קורס, נסה את הפעולות הבאות:

- אם אתה משתמש ביישום שולחן העבודה של Teams, [ודא שהיישום מעודכן במלואו](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- ודא שכל [כתובות ה-url וטווחי הכתובות של Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) נגישים.

- התחבר עם חשבון מנהל הדיירים שלך ובדוק את [לוח הבקרה של שירות בריאות](https://docs.microsoft.com/office365/enterprise/view-service-health) כדי לוודא כי אין הפסקת או השפלה שירות קיים.

- הסרת התקנה והתקנה מחדש של יישום הצוותים (קישור)
    - דפדף אל התיקיה%Appdata%\ute\cos\n במחשב שלך ומחק את כל הקבצים בספריה זו.
    - [הורד והתקן את יישום הצוותים](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), ואם אפשר, התקן צוותים כמנהל (לחץ לחיצה ימנית על תוכנית ההתקנה של הצוותים ובחר באפשרות "הפעל כמנהל" אם הוא זמין).

אם לקוח הצוותים שלך עדיין מתרסק, האם תוכל לשחזר את הבעיה? אם כן:

1. השתמש במקליט השלבים כדי ללכוד את הצעדים שלך.
    - סגור את כל היישומים המיותרים או הסודיים.
    - הפעל את מקליט השלבים ושנה את הבעיה בזמן שהתחברת עם חשבון המשתמש המושפע.
    - [לאסוף את יומני הצוותים כי ללכוד את הצעדים המוקלט כי](https://docs.microsoft.com/microsoftteams/log-files). **הערה**: ודא שלכדת את כתובת הכניסה של המשתמש המושפעים.
    - לאסוף את הקובץ dump ו/או מידע דלי תקלות (Windows). הפעל את Windows Powershell במחשב שבו ההתרסקות מתרחשת ולהפעיל את הפקודות הבאות:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. צרף את הקובץ לתיק התמיכה שלך.
