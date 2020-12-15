---
title: אין תוצאות המוחזרות במהלך חיפוש תוכן/ייצוא
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/14/2020
ms.locfileid: "49678677"
---
# <a name="no-results-returned-during-content-searchexport"></a>אין תוצאות המוחזרות במהלך חיפוש תוכן/ייצוא

אם אתה נתקל בבעיות בתרחישים הבאים של גילוי אלקטרוני:

- חיפוש תוכן/ייצוא מחזיר נתונים או נתונים בלתי צפויים
- חיפוש הגילוי אלקטרוני או הייצוא נכשלים

ייתכן שהסיבה לכך היא מסנני אבטחה מסוימים המוגדרים על-ידי מנהל מערכת ספציפי ושאינם מועברים לכל מנהלי המערכת.

כדי לפתור זאת, בדוק אם קיימים מסנני אבטחה של תאימות שעשויים לגרום לבעיות אלה:

1. התחברות למרכז האבטחה והתאימות של Powershell
2. הפעלת הcommandlet הבאים:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

לקבלת מידע נוסף אודות מסנני אבטחה של תאימות, ראה [סינון הרשאות עבור חיפוש תוכן](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
