---
title: Teams לקוח קורס
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
ms.openlocfilehash: bef16351b55ac4765539d66ab86a71183f66f0dd
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321626"
---
# <a name="teams-client-crashing"></a>Teams לקוח קורס

אם לקוח Teams שלך קורס, נסה את הפעולות הבאות:

- אם אתה משתמש ביישום שולחן העבודה של Teams, [ודא שהיישום מעודכן במלואו](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- ודא שכל כתובות [Microsoft 365 וטווחי הכתובות](https://docs.microsoft.com/microsoftteams/connectivity-issues) נגישים.

- היכנס באמצעות חשבון מנהל הדייר שלך ובדוק את לוח [המחוונים](https://docs.microsoft.com/office365/enterprise/view-service-health) של תקינות השירות כדי לוודא שלא קיימים בעיות של מחסור או שפלת שירות.

- הסרת התקנה והתקנה מחדש של Teams היישום
    - עבור אל התיקיה %appdata%\Microsoft\Teams\ במחשב שלך ומחק את כל הקבצים במדריך כתובות זה.
    - [הורד והתקן את יישום Teams](https://www.microsoft.com/microsoft-teams/download-app), ואם הדבר אפשרי, התקן Teams כמנהל מערכת (לחץ באמצעות לחצן העכבר הימני על Teams תוכנית ההתקנה ובחר **הפעל** כמנהל מערכת אם זמין).

אם Teams שלך עדיין קורס, נסה לשחזר את הבעיה. אם תוכל:

1. השתמש במקליט השלבים כדי ללכוד את השלבים שלך.
    - סגור את ALL יישומים לא נחוצים או סודיים.
    - הפעל את מקליט השלבים ושכפול הבעיה בעת כניסה באמצעות חשבון המשתמש המושפע.
    - [אסוף את יומני הרישום של הצוותים שלכודים את שלבי השכפול המוקלטים.](https://docs.microsoft.com/microsoftteams/log-files) 
    
    **הערה:** הקפד ללכוד את כתובת הכניסה של המשתמש מושפע.
    - אסוף את פרטי ה- dump ו/או הדלי של תקלות (Windows). הפעל Windows Powershell במחשב שבו מתרחשת קריסה ולהפעיל את הפקודות הבאות (לאחר כל פקודה, הקש Enter):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. לאחר יצירת קובץ הטקסט ומופיע על המסך, שמור את הקובץ וצרף אותו לבקשת השירות. 
