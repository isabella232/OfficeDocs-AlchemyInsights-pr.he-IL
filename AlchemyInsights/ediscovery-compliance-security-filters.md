---
title: לא הוחזרו תוצאות במהלך חיפוש/ייצוא של תוכן
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
ms.openlocfilehash: 5c04364f98dccbcad0f011df866f137d79c166ad3839b408d6be447d50a87ac3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101267"
---
# <a name="no-results-returned-during-content-searchexport"></a>לא הוחזרו תוצאות במהלך חיפוש/ייצוא של תוכן

אם אתה נתקל בבעיות בתרחישים הבאים של גילוי אלקטרוני:

- חיפוש/ייצוא תוכן לא מחזיר נתונים או נתונים בלתי צפויים
- חיפוש גילוי אלקטרוני או ייצוא נכשלים

ייתכן שהנו עקב מסנני אבטחה מסוימים של תאימות שהוגנו על-ידי מנהל מערכת ספציפי ולא הועברו לכל מנהלי המערכת.

כדי לפתור בעיה זו, בדוק אם זמינים מסנני אבטחה של תאימות שעשויים לגרום לבעיות אלה:

1. התחברות ל- Powershell של מרכז האבטחה והתאימות
2. הפעל את הפקודות הבאות:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

לקבלת מידע נוסף אודות מסנני אבטחת תאימות, [ראה סינון הרשאות עבור חיפוש תוכן](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
