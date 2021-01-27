---
title: בעיות גישה מותנית
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014882"
---
# <a name="conditional-access-issues"></a>בעיות גישה מותנית

**פתרון בעיות באבחון הכניסה**

באפשרותך לגלות במהירות מה קרה או לאבחן בעיות הקשורות לכניסה למשתמש באמצעות [אבחון הכניסה](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):

1. הפעל את אבחון הכניסה.
1. אתר את האירוע לניתוח על-ידי הזנת הפרטים שאתה משתמש בהם לגבי המשתמש, היישום, זמן הכניסה, מזהה הבקשה או מזהה המתאם.
1. סקור את תוצאות האבחון המציגות את הפרטים של מה שקרה ואילו פעולות ניתן לבצע כדי לבצע שינויים (אם נדרשים שינויים כלשהם).

**שלבים לפתרון בעיות בכניסה** 

1. נווט אל דף הכניסה של תכלת לספירה.
1. הוסף כניסה למסנן לפי משתמש, טווח זמן, יישום, מצב, יישום לקוח וכן הלאה.
1. בחר אירוע כניסה והצג את הכרטיסיה ' גישה מותנית ' כדי לראות אילו פריטי מדיניות הוערכו.
1. לחץ על השורה של מדיניות כדי להציג את פרטי המדיניות ולהבין מדוע היא הוחלה.

**כלים לפתרון בעיות במדיניות גישה מותנית**

- מצב דוח בלבד מאפשר לך להעריך מדיניות מבלי להשפיע על משתמשים.
- כלי ' מה-אם ' מאפשר לך לדמות אירועי כניסה ולראות אילו פריטי מדיניות חלים.
- התובנות והדוחות של חוברת העבודה מציגות השפעה בזמן אמת על כל מדיניות.

**מדיניות הגנה בסיסית**

מדיניות הגנה בסיסית לא אושרה. הם אינם נאכפים עוד ויוסרו בקרוב מפורטל התכלת. אנו ממליצים לאפשר [ברירות מחדל של אבטחה](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

לקבלת מידע נוסף אודות גישה מותנית, ראה:

[שיטות עבודה מומלצות לגישה מותנית ב-תכלת Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [תנאים בגישה](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 מותנית [פקדים בגישה](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 מותנית [מיקומים בגישה מותנית](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
