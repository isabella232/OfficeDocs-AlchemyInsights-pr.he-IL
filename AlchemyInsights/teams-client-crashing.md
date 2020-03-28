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
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030582"
---
# <a name="teams-client-crashing"></a>לקוח Teams קורס?

אם לקוח Teams שלך קורס, נסה את הפעולות הבאות:

- אם אתה משתמש ביישום שולחן העבודה של Teams, [ודא שהיישום מעודכן במלואו](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- ודא שכל [כתובת ה-URL של Office 365 וטווחי הכתובות](https://docs.microsoft.com/microsoftteams/connectivity-issues) נגישים.

- היכנס עם חשבון מנהל המערכת שלך ובדוק את [לוח המחוונים של תקינות השירות](https://docs.microsoft.com/office365/enterprise/view-service-health) כדי לאמת שלא קיימות הפסקות חשמל או ירידה בביצועי השירות.

 - כצעד אחרון, באפשרותך לנסות לנקות את המטמון של לקוח Teams:

    1.  צא לחלוטין מלקוח שולחן העבודה של Microsoft Teams. באפשרותך ללחוץ בעזרת לחצן העכבר הימני על **Teams** מתוך מגש הסמל וללחוץ על **צא**, או להפעיל את מנהל המשימות ולעצור לגמרי את התהליך.

    2.  עבור אל סייר הקבצים והקלד %appdata%\Microsoft\teams.

    3.  לאחר שתיכנס אל מדריך הכתובות, תראה כמה מהתיקיות הבאות:

         - מתוך **מטמון יישום**, עבור אל מטמון ומחק את כל הקבצים במיקום המטמון:  %appdata%\Microsoft\teams\application cache\cache.

        - מתוך **Blob_storage**, מחק את כל הקבצים: %appdata%\Microsoft\teams\blob_storage.

        - מתוך **מטמון**, מחק את כל קבצים: %appdata%\Microsoft\teams\Cache.

        - מתוך **מסדי נתונים**, מחק את כל קבצים: %appdata%\Microsoft\teams\Cache.

        - מתוך **GPUCache**, מחק את כל קבצים: %appdata%\Microsoft\teams\Cache.

        - מתוך **IndexedDB**, מחק את קובץ ה-.db: %appdata%\Microsoft\teams\IndexedDB.

        - מתוך **אחסון מקומי**, מחק את כל הקבצים: %appdata%\Microsoft\teams\Local Storage.

        - לבסוף, מתוך **tmp**, מחק את כל קבצי: %appdata%\Microsoft\teams\tmp.

    4. הפעל מחדש את לקוח Teams שלך.
