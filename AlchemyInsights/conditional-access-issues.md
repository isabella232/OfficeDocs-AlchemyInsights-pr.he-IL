---
title: בעיות גישה מותות
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
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069965"
---
# <a name="conditional-access-issues"></a>בעיות גישה מותות

**פתרון בעיות באבחון הכניסה**

באפשרותך לגלות במהירות מה קרה או לאבחן בעיות הקשורות להכניסה של המשתמש באמצעות אבחון [הכניסה](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):

1. הפעל את אבחון הכניסה.
1. אתר את האירוע שיש לנתח על-ידי הזנת הפרטים שיש לך לגבי המשתמש, היישום, זמן הכניסה, מזהה הבקשה או מזהה המתאם.
1. סקור את תוצאות האבחון המציגות את הפרטים של מה שקרה ואת הפעולות שתוכל לבצע כדי לבצע שינויים (אם נדרשים שינויים כלשהם).

**שלבים לפתרון בעיות של כניסה** 

1. נווט אל דף הכניסה של Azure AD.
1. סינון הכניסה לפי משתמש, טווח זמן, יישום, מצב, יישום לקוח, וכך הלאה.
1. בחר אירוע כניסה וצפה בכרטיסיה Access תנאי כדי לראות אילו פריטי מדיניות הוערכים.
1. לחץ על השורה של מדיניות כדי להציג את פרטי המדיניות ולהבין מדוע היא הוחלה.

**כלים לפתרון בעיות של מדיניות Access מותנות**

- מצב דוח בלבד מאפשר לך להעריך מדיניות מבלי להשפיע על המשתמשים.
- כלי מה-אם מאפשר לך לדמות אירועי כניסה ולראות אילו פריטי מדיניות חלים.
- תובנות העבודה והדיווח מציגות השפעה בזמן אמת על כל מדיניות.

**מדיניות הגנה בסיסית**

פריטי מדיניות של הגנה בסיסית נותק. הם לא נאכפים עוד והם יוסרו בקרוב מפורטל Azure. מומלץ להפוך ברירות [מחדל של אבטחה לאפשרות](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

לקבלת מידע נוסף אודות תנאי Access ראה:

[שיטות עבודה מומלצות לגישה מותית ב- Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [תנאים בתנאי Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [פקדים ב' Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [מיקומים ב' Access](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
