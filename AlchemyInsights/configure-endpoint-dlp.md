---
title: קביעת תצורה של DLP של נקודת קצה
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402425"
---
# <a name="configure-endpoint-dlp"></a>קביעת תצורה של DLP של נקודת קצה

Microsoft Endpoint DLP מאפשר לך להרחיב את יכולת ההגנה והניטור של DLP למידע רגיש במכשירי Windows 10. לאחר שהמכשירים מחוברים לניהול מכשירים, ניתן ליצור פריטי מדיניות DLP כדי לאכוף פעולות הגנה על פריטים. ניתן להשתמש בסייר הפעילות כדי לנטר פעילות עבור פריטים רגישים. לקבלת מידע נוסף, ראה [צירוף מכשירים לניהול מכשירים](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

כדי להתחיל בעבודה עם DLP בנקודת קצה:

- ודא שיש לך את רישוי ה- SKU/המנויים המתאימים. לקבלת מידע נוסף, ראה [רישוי SKU/מנויים](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- בדוק את ההרשאות הדרושות כדי להפוך את ניהול המכשירים לזמין, לגשת לדף הצירוף או להפעיל/לכבות ניטור אחר מכשירים. לקבלת מידע נוסף, ראה [הרשאות](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- צרף מכשירים לניהול מכשירים על-ידי ביצוע ההליך לצירוף מכשירים. אם האפשרות 'צירוף מכשיר (תצוגה מקדימה)' חסרה לך ב **הגדרות** תאימות M365, אשר שיש לך את הרשיון וההרשאות המתאימים שאליהם מתייחסת ההפניה לעיל. לקבלת מידע נוסף, ראה [צירוף מכשירים](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- צור פריטי מדיניות DLP כדי להגן על פריטים רגישים. לקבלת מידע, ראה [תרחישי מדיניות DLP של נקודת קצה](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).

לקבלת מידע נוסף על DLP בנקודת הקצה של Microsoft, ראה [קבל מידע נוסף על מניעת אובדן נתונים (תצוגה מקדימה) של נקודת קצה של Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**שלבי איסוף נתונים חשובים, אם יש צורך בתמיכה:**

1. הורד תצוגה מקדימה של MDATP Client Analyzer מ- [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")
2. הפעל את הכלי כמנהל מערכת מחלון ה- cmd:
3. MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t
4. כאשר תופיעה הבקשה "הקלד את מספר הדקות לאיסוף מעקבים: ", הזן את מספר הדקות הדרושות כדי להפעיל את התרחיש
5. הפעל את התרחיש

אסוף את פלט קובץ ה- Zip שיינתן לסוכן התמיכה.
