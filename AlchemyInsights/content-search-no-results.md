---
title: חיפוש תוכן ללא תוצאות
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
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680648"
---
# <a name="no-results-from-content-searchexports"></a>אין תוצאות מחיפוש תוכן/ייצוא

בעיות בחיפוש תוכן/הייצוא לא מחזירות נתונים עשויים לנבוע ממסנן אבטחת תאימות מסוים שהיה הגדרה על-ידי מנהל מערכת ספציפי, ולא לקיים תקשורת עם כל מנהלי המערכת.

כדי לפתור זאת, בדוק אם קיימים מסנני אבטחה של תאימות שעשויים לגרום לכך:
1. התחברות למרכז האבטחה והתאימות של Powershell
2. הפעלת הcommandlet הבאים:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-ארגון $org