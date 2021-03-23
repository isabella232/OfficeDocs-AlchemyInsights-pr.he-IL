---
title: פינוי שטח כונן ב-Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036586"
---
# <a name="free-up-drive-space-in-windows-10"></a>פינוי שטח כונן ב-Windows 10

להלן שתי אפשרויות כדי לפנות שטח כונן ב-Windows:

- פנה שטח כונן ב-Windows 10.
- פנה מקום עבור עדכונים של Windows 10 עם התקן אחסון חיצוני.

אם עדיין יש לך שטח דיסק נמוך לאחר השימוש בניקוי הדיסק, ייתכן שהתיקיה Temp מתעוררת במהירות באמצעות קבצי יישום (. appx) המשמשים את Microsoft Store. כדי לפתור בעיה זו, אפס את החנות, נקה את מטמון החנות ולאחר מכן הפעלת פותר הבעיות של Windows Update. ודא ש-Microsoft Store סגור לפני שתמשיך בשלבים אלה.

**שלב 1: איפוס Microsoft Store**

**הערה** פעולה זו מוחקת לצמיתות את נתוני האפליקציה במכשיר, כולל העדפותיך ופרטי הכניסה.

1. בחר באפשרות **התחל**  >  **הגדרות**  >  **אפליקציות**  >  של **אפליקציות &**.

1. ברשימת האפליקציות, אתר ובחר חנות Microsoft.

1. בחר **אפשרויות מתקדמות**.

1. גלול מטה ובחר **איפוס** ולאחר מכן **אשר את איפוס**.

**שלב 2: ניקוי מטמון חנות Microsoft**

1. הקש על מקש סמל Windows + R כדי לפתוח את תיבת הדו ההפעלה.

1. הקלד wsreset.exe **ובחר אישור**.

1. נפתח חלון שורת פקודה ריקה. לאחר כ-10 שניות, החלון נסגר והחנות נפתחת באופן אוטומטי.

**שלב 3: אפס את Windows Update**

1. בחר **התחל**  >  עדכון **הגדרות &**  >    >  **פתרון בעיות** אבטחה.

1. גלול מטה ובחר **Windows Update** מהרשימה ובחר **הפעלת פותר הבעיות**.

1. אתחל מחדש את המחשב ובדוק אם אתה עדיין נתקל בבעיה.

