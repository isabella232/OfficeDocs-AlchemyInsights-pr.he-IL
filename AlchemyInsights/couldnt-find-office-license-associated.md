---
title: תיקון יישומי Microsoft 365 לא הצליח למצוא הודעה משויכת של רשיונות Office
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
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816489"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>תיקון ההודעה של יישומי Microsoft 365 "לא היתה אפשרות למצוא רשיונות Office משויכים"

אם אתה מקבל הודעה זו, נסה את הפעולות הבאות:

1. בדוק את הגדרות חומת האש, תוכנת האנטי-וירוס וה- Proxy כדי לוודא שהם אינם חוסמים גישה לאינטרנט לאפליקציות Microsoft 365. ראה [כתובות URL וטווחי כתובות IP של Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. הסר [והקצה מחדש את רשיון Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) עבור המשתמש המושפע. 
3. פתח יישום Office [והירשם](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) מחשבונות משתמשים קיימים.
4. עבור אל הגדרות Windows > **חשבונות**  >  **דואר אלקטרוני &** והסר את כל חשבונות העבודה למעט החשבון המושפע.
5. עבור אל הגדרות Windows > **חשבונות** Access בעבודה או  >  **בבית ספר**, ונתק את כל חשבונות העבודה למעט החשבון המושפע.
6. איפוס מצב ההפעלה של Office. [למד כיצד לעשות זאת](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [היכנס באמצעות](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) חשבון המשתמש המושפע.

לקבלת פתרונות נוספים לפתרון בעיות, ראה שגיאות מוצר ללא רשיון [ושגיאות הפעלה ב- Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).