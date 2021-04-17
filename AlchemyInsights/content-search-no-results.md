---
title: חיפוש תוכן ללא תוצאות
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
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816849"
---
# <a name="no-results-from-content-searchexports"></a>אין תוצאות מחיפוש/ייצוא תוכן

בעיות בחיפוש/ייצוא תוכן עשויות שלא להחזיר נתונים עקב מסנן אבטחה מסוים של תאימות שהוגנה על-ידי מנהל מערכת ספציפי ולא העברתם לכל מנהלי המערכת.

כדי לפתור בעיה זו, בדוק אם זמינים מסנני אבטחה של תאימות שעשויים לגרום לכך:
1. התחברות למרכז האבטחה והתאימות Powershell
2. הפעל את הפקודות הבאות:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org