---
title: כלי אבחון השירות עבור Windows Virtual Desktop
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: 58688e3216ba6777b1a4f76095bd39c81a2d2a8294e06b6bc61c7134f6d589f9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052387"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>כלי אבחון השירות עבור Windows Virtual Desktop

Windows Virtual Desktop (WVD) מציע כלי אבחון המאפשר למנהלי מערכת לזהות שגיאות באמצעות ממשק יחיד. כלי זה מבצע רישום של מידע הקשור לאבחון בכל פעם שמישהו שהוקצה לו תפקיד WVD משתמש ב- WVD. כל יומן רישום מכיל מידע אודות תפקיד WVD המעורב בפעילות, הודעות השגיאה המופיעות במהלך ההפעלה ומידע אודות הדייר והמשתמש. ניתן לקבוע את תצורת Azure Log Analytics כדי ללכוד את יומן הפעילות שנוצר על-ידי כלי האבחון. כך ניתן לעשות זאת:

1. יצירת סביבת עבודה של Log Analytics עם פורטל [Azure או](https://go.microsoft.com/fwlink/?linkid=2129500) [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [התחברות Windows מחשבים לצג Azure](https://go.microsoft.com/fwlink/?linkid=2129913). קבל את מזהה סביבת העבודה ואת המפתח הראשי של סביבת העבודה שלך. אשף ההגדרה זקוק למידע זה כדי להגדיר כראוי את הסוכן ולהבטיח שהוא יוכל לקיים תקשורת עם Azure Monitor.
1. [העברת נתוני אבחון לסביבת העבודה שלך](https://go.microsoft.com/fwlink/?linkid=2128284). באפשרותך לדחוף נתוני אבחון מהדייר WVD שלך ל- Log Analytics עבור סביבת העבודה שלך.
1. [זהה ואבחן בעיות](https://go.microsoft.com/fwlink/?linkid=2128338) פנימיות או חיצוניות ביחס ל- WVD.

לקבלת מידע נוסף אודות קביעת התצורה של כלי אבחון השירות עבור WVD, ראה [שימוש ב- Log Analytics עבור תכונת האבחון](https://go.microsoft.com/fwlink/?linkid=2128084).
