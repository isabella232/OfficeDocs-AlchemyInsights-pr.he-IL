---
title: אין תוצאות חיפוש של תוכן
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516780"
---
# <a name="no-results-from-content-searchexports"></a>אין תוצאות מתוך תוכן החיפוש/ייצוא

בעיות עם תוכן החיפוש/ייצוא אינה מחזירה נתונים עשוי לנבוע מסנן אבטחה מסוימים תאימות שהיה ההתקנה על-ידי Admin ספציפיים והעברה לא אותה על כל המנהלים.

כדי לפתור בעיה זו, בדוק אם ישנם מסננים אבטחה תאימות עלולות לגרום זו:
1. להתחבר Powershell מרכז תאימות ואבטחה
2. הפעל את commandlets הבאות:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-$org של הארגון