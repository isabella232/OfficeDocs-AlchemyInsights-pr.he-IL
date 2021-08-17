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
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058003"
---
# <a name="no-results-from-content-searchexports"></a>אין תוצאות מחיפוש/ייצוא תוכן

בעיות בחיפוש/ייצוא תוכן עשויות שלא להחזיר נתונים עקב מסנן אבטחה מסוים של תאימות שהוגנה על-ידי מנהל מערכת ספציפי ולא העברתם לכל מנהלי המערכת.

כדי לפתור בעיה זו, בדוק אם זמינים מסנני אבטחה של תאימות שעשויים לגרום לכך:
1. התחברות ל- Powershell של מרכז האבטחה והתאימות
2. הפעל את הפקודות הבאות:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org