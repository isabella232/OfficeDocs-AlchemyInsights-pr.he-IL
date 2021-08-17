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
ms.openlocfilehash: 4a4dbd60f98e86cf2a4d861a763f75ada04f9e500164c01cb858a1537148a62f
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892800"
---
# <a name="configure-endpoint-dlp"></a>קביעת תצורה של DLP של נקודת קצה

Microsoft Endpoint DLP מאפשר לך להרחיב את יכולת ההגנה והניטור של DLP למידע רגיש במכשירי Windows 10. לאחר שהמכשירים מחוברים לניהול מכשירים, ניתן ליצור פריטי מדיניות DLP כדי לאכוף פעולות הגנה על פריטים. ניתן להשתמש בסייר הפעילות כדי לנטר פעילות עבור פריטים רגישים. לקבלת מידע נוסף, ראה [צירוף מכשירים לניהול מכשירים](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

כדי להתחיל בעבודה עם DLP בנקודת קצה:

- ודא שיש לך את רישוי ה- SKU/המנויים המתאימים. לקבלת מידע נוסף, ראה [רישוי SKU/מנויים](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- בדוק את ההרשאות הדרושות כדי להפוך את ניהול המכשירים לזמין, לגשת לדף הצירוף או להפעיל/לכבות ניטור אחר מכשירים. לקבלת מידע נוסף, ראה [הרשאות](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- צרף מכשירים לניהול מכשירים על-ידי ביצוע ההליך לצירוף מכשירים. לקבלת מידע נוסף, ראה [צירוף מכשירים](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- צור פריטי מדיניות DLP כדי להגן על פריטים רגישים. לקבלת מידע, ראה [תרחישי מדיניות DLP של נקודת קצה](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

לקבלת מידע נוסף על DLP בנקודת הקצה של Microsoft, ראה [קבל מידע נוסף על מניעת אובדן נתונים (תצוגה מקדימה) של נקודת קצה של Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**שלבי איסוף נתונים חשובים, אם יש צורך בתמיכה:**

1. הורד [את MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).
1. הפעל את הכלי כמנהל מערכת מחלון ה- cmd:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. כאשר תתבקש לעשות **זאת באמצעות הזן את מספר הדקות לאיסוף מעקבים:**, הזן את מספר הדקות הדרוש כדי להפעיל את התרחיש.
1. הפעל את התרחיש.

אסוף את פלט קובץ ה- Zip כדי להעניק לסוכן התמיכה.
