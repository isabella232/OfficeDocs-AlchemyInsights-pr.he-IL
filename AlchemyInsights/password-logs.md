---
title: יומני סיסמאות
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50525139"
---
# <a name="password-logs"></a>יומני סיסמאות

**אני נתקל בבעיות בגישה ליומני ביקורת של איפוס סיסמאות**

כדי לפתור בעיות בנוגע לגישה ליומני ביקורת של איפוס סיסמאות, בצע את השלב הבא:

ודא שאתה מורשה להציג יומני ביקורת. 

רק התפקידים הבאים מורשים:
 - מנהל מערכת כללי
 - מנהל מערכת של אבטחה
 - קורא האבטחה

**אני מעוניין לראות את כל אירועי הביקורת של איפוס הסיסמאות מהזמן שאני מפרוס לראשונה**

מתבצעת העברה של עד 120,000 סיסמאות לאיפוס הסיסמה/הרישום מאוחסנים בדוחות של 30 הימים האחרונים. מגבלה מרבית זו חלה על ממשק המשתמש בעת הורדת ה-CSV. אירועי 1,000,000 זמינים דרך PowerShell.
לקבלת מידע נוסף, עיין בקישורים הבאים:

- [אירועי איפוס סיסמה בשירות עצמי מתוך API של דוחות ואירועים של ' תכלת ואירועים '](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [כיצד להוריד את אירועי הרישום לאיפוס סיסמה במהירות באמצעות PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**אני מעוניין להבין עוד אודות יכולות דיווח של איפוס סיסמאות**

בדוק מי נרשם או מאפס סיסמאות באמצעות האפשרות ' איפוס סיסמה של הודעות מיידיות ' בפורטל ' תכלת ' תחת ' **משתמשים וקבוצות**'.
לקבלת מידע נוסף, עיין בקישורים הבאים:

- [מבט כולל על דוחות איפוס סיסמה](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [כיצד להציג דוחות של איפוס סיסמאות בפורטל התכלת](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [אירועי איפוס סיסמה בשירות עצמי מתוך API של דוחות ואירועים של ' תכלת ואירועים '](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [כיצד להוריד את אירועי הרישום לאיפוס סיסמה במהירות באמצעות PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


