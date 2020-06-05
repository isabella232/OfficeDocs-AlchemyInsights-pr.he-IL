---
title: תיקון יישומים 365 של Microsoft לא היתה למצוא הודעה המשויכת לרשיונות משרדיים
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 65ffae1a784f841cb08a5df52b02671a4526d9d4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580442"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>תיקון האפליקציות של Microsoft 365 "לא היתה משויכת לרשיונות משרדיים" הודעה

אם תקבל הודעה זו, נסה את הפעולות הבאות:

1. בדוק את חומת האש, תוכנת האנטי-וירוס והגדרות ה-proxy כדי לוודא שהן אינן חוסמות גישה לאינטרנט ל-Microsoft 365 apps. ראה [כתובות url וטווחי כתובות IP של Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. הסר [והקצה מחדש את רשיון Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) עבור המשתמש המושפע. 
3. פתח יישום Office [והיכנס](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) מחשבונות משתמשים קיימים.
4. עבור אל הגדרות Windows _ gt_ **חשבונות**  >  **דואר אלקטרוני _ amp_ חשבונות**, והסר את כל חשבונות העבודה מלבד החשבון המושפע.
5. עבור אל הגדרות Windows _ **Accounts**  >  **העבודה של הגישה לחשבונות או לבית הספר**, ונתק את כל חשבונות העבודה מלבד החשבון המושפע.
6. איפוס מצב ההפעלה של Office. [למד כיצד לעשות זאת](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [היכנס](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) באמצעות חשבון המשתמש המושפע.

לקבלת פתרונות נוספים לפתרון בעיות, ראה [שגיאות מוצר והפעלה לא מורשה ב-Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).