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
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800378"
---
# <a name="no-results-from-content-searchexports"></a>אין תוצאות מתוך תוכן החיפוש/ייצוא

בעיות עם תוכן החיפוש/ייצוא אינה מחזירה נתונים עשוי לנבוע מסנן אבטחה מסוימים תאימות שהיה ההתקנה על-ידי Admin ספציפיים והעברה לא אותה על כל המנהלים.

כדי לפתור בעיה זו, בדוק אם ישנם מסננים אבטחה תאימות עלולות לגרום זו:
1. להתחבר Powershell מרכז תאימות ואבטחה
2. הפעל את commandlets הבאות:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-$org של הארגון