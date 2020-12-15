---
title: כלי אבחון שירות עבור שולחן העבודה של Windows Virtual
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
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/14/2020
ms.locfileid: "49678621"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>כלי אבחון שירות עבור שולחן העבודה של Windows Virtual

שולחן העבודה של Windows Virtual (WVD) מציע כלי אבחון המאפשר למנהלי מערכת לזהות שגיאות באמצעות ממשק יחיד. כלי זה מבצע רישום של מידע הקשור לאבחון כאשר WVD נמצא בשימוש על-ידי משתמש שהוקצה לו תפקיד WVD. כל יומן מכיל מידע על תפקיד WVD המעורב בפעילות, הודעות השגיאה המופיעות במהלך ההפעלה והמידע אודות הדייר והמשתמש. ניתן לקבוע את התצורה של ניתוח יומן הרישום של תכלת כדי ללכוד את יומן הפעילות שנוצר על-ידי כלי האבחון. כך ניתן לעשות זאת:

1. צור סביבת עבודה של ניתוח יומני רישום עם [הפורטל ' תכלת](https://go.microsoft.com/fwlink/?linkid=2129500) ' או ' [תכלת PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501)'.
1. [חבר את מחשבי Windows למסך התכלת](https://go.microsoft.com/fwlink/?linkid=2129913). קבל את מזהה סביבת העבודה ואת המפתח הראשי של סביבת העבודה שלך. אשף ההתקנה זקוק למידע זה כדי לקבוע את תצורת הסוכן כראוי וכדי להבטיח שהוא יוכל לקיים תקשורת עם צג התכלת.
1. [דחיפת נתוני אבחון לסביבת העבודה שלך](https://go.microsoft.com/fwlink/?linkid=2128284). באפשרותך לדחוף נתוני אבחון מדייר WVD לניתוח יומן הרישום עבור סביבת העבודה שלך.
1. [זיהוי ואבחון של בעיות](https://go.microsoft.com/fwlink/?linkid=2128338) פנימיות או חיצוניות ביחס לWVD.

לקבלת מידע נוסף אודות קביעת התצורה של כלי אבחון השירות עבור WVD, ראה [שימוש בניתוח יומני רישום עבור התכונה ' אבחון](https://go.microsoft.com/fwlink/?linkid=2128084)'.
