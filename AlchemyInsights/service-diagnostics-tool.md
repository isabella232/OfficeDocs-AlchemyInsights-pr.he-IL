---
title: כלי אבחון השירות עבור Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595860"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>כלי אבחון השירות עבור Windows Virtual Desktop

Windows Virtual Desktop (WVD) מציע כלי אבחון המאפשר למנהלי מערכת לזהות שגיאות באמצעות ממשק יחיד. כלי זה מבצע רישום של מידע הקשור לאבחון בכל פעם שמישהו שהוקצה לו תפקיד WVD משתמש ב- WVD. כל יומן רישום מכיל מידע אודות תפקיד WVD המעורב בפעילות, הודעות השגיאה המופיעות במהלך ההפעלה ומידע אודות הדייר והמשתמש. ניתן לקבוע את תצורת Azure Log Analytics כדי ללכוד את יומן הפעילות שנוצר על-ידי כלי האבחון על-ידי ביצוע השלבים הבאים:

1. יצירת סביבת עבודה של Log Analytics עם פורטל [Azure או](https://go.microsoft.com/fwlink/?linkid=2129500) [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).

1. [חבר מחשבי Windows לצג Azure](https://go.microsoft.com/fwlink/?linkid=2129913). קבל את מזהה סביבת העבודה ואת המפתח הראשי של סביבת העבודה שלך. אשף ההגדרה זקוק למידע זה כדי להגדיר כראוי את הסוכן ולהבטיח שהוא יוכל לקיים תקשורת עם Azure Monitor.

1. [העברת נתוני אבחון לסביבת העבודה שלך](https://go.microsoft.com/fwlink/?linkid=2128284). באפשרותך לדחוף נתוני אבחון מהדייר WVD שלך ל- Log Analytics עבור סביבת העבודה שלך.

1. [זהה ואבחן](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) בעיות פנימיות או חיצוניות ביחס ל- WVD.

לקבלת מידע נוסף אודות קביעת התצורה של כלי אבחון השירות עבור WVD, ראה שימוש ב- Log Analytics עבור תכונת האבחון.