---
title: DLP של נקודת קצה לא נפרס במכשיר של המשתמש
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731585"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>DLP של נקודת קצה לא נפרס במכשיר של המשתמש

אם ההגדרה מניעת אובדן נתונים של נקודת קצה (DLP) לא חלה על מכשיר של משתמש, אשר שאתה מביע את הדרישות הבאות:

- Windows 10 x64 גירסת Build מס' 1809 ואילך מותקנת במכשיר.
- לקוח נגד תוכנות זדוניות גירסה 4.18.2009.7 ואילך מותקן.
- המכשיר הוא **אחד** מאלה:
    
    - Azure Active Directory (Azure AD) מצורף
    - Azure AD היברידי מצורף
    - AAD רשום

- כדי לאכוף פעולות מדיניות, ודא שדפדפן Microsoft Chromium Edge מותקן במכשיר נקודת הקצה.

לקבלת דרישות נוספות לפריסת DLP של נקודת קצה, ראה [תחילת העבודה עם מניעת אובדן נתונים של נקודת קצה](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).