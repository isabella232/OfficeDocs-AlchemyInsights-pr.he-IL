---
title: תיקון יישומי Microsoft 365 לא מצליח למצוא הודעה המשויכת לרשיונות office
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
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747696"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>תיקון יישומי Microsoft 365 "לא היתה אפשרות למצוא את ההודעה" רשיונות office משויכים "

אם אתה מקבל הודעה זו, נסה את הפעולות הבאות:

1. בדוק את חומת האש, תוכנת האנטי-וירוס והגדרות ה-proxy כדי לוודא שהם אינם חוסמים את הגישה לאינטרנט ליישומי Microsoft 365. ראה [כתובות url וטווחי כתובות IP של Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. הסר [והקצה מחדש את רשיון Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) עבור המשתמש המושפע. 
3. פתח יישום של Office [וצא](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) מחשבונות משתמשים קיימים.
4. עבור אל Windows Settings > **חשבונות**  >  **דואר אלקטרוני & חשבונות**והסר את כל חשבונות העבודה למעט החשבון המושפע.
5. עבור אל הגדרות Windows Settings > **חשבונות**  >  **גישה לעבודה או לבית הספר**, ונתק את כל חשבונות העבודה למעט החשבון המושפע.
6. איפוס מצב ההפעלה של Office. [למד כיצד לעשות זאת](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [היכנס](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) באמצעות חשבון המשתמש המושפע.

לקבלת פתרונות נוספים לפתרון בעיות, ראה [שגיאות מוצר ללא רשיון והפעלה ב-Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).