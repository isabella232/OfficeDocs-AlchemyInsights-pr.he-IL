---
title: פינוי שטח בכונן ב- Windows 10
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
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505357"
---
# <a name="free-up-drive-space-in-windows-10"></a>פינוי שטח בכונן ב- Windows 10

להלן שתי אפשרויות לפינוי שטח בכונן ב- Windows:

- פנה שטח בכונן ב- Windows 10.
- פנה שטח עבור עדכוני Windows 10 באמצעות התקן אחסון חיצוני.

אם עדיין יש לך שטח דיסק מועט לאחר השימוש ב'ניקוי דיסק', ייתכן שתיקיית Temp מתמלאת במהירות בקבצי אפליקציה (appx.) המשמשים את Microsoft Store. כדי לפתור בעיה זו, אפס את ה- Store, נקה את מטמון ה- Store ולאחר מכן הפעל את פותר הבעיות של Windows Update. ודא ש- Microsoft Store סגורה לפני שתמשיך לביצוע שלבים אלה.

**שלב 1: איפוס Microsoft Store**

**הערה** פעולה זו תמחק לצמיתות את נתוני האפליקציה במכשיר, כולל ההעדפות ופרטי הכניסה.

1. בחר **התחל** > **הגדרות** > **אפליקציות** > **אפליקציות ותכונות**.

1. ברשימת האפליקציות, אתר ובחר את Microsoft Store.

1. בחר **אפשרויות מתקדמות**.

1. גלול מטה ובחר באפשרות **איפוס** ולאחר מכן **אשר איפוס**.

**שלב 2: ניקוי המטמון של Microsoft Store**

1. הקש על מקש סמל Windows + ‏R כדי לפתוח את תיבת הדו-שיח 'הפעלה'.

1. הקלד wsreset.exe ובחר באפשרות **אישור**.

1. נפתח חלון ריק של שורת פקודה. לאחר כ- 10 שניות, החלון ייסגר וה- Store תיפתח באופן אוטומטי.

**שלב 3: איפוס Windows Update**

1. בחר **התחל** > **הגדרות** > **עדכון ואבטחה** > **פתרון בעיות**.

1. גלול מטה ובחר את **Windows Update** מהרשימה ולאחר מכן בחר באפשרות **הפעל את פותר הבעיות**.

1. אתחל מחדש את המחשב ובדוק אם אתה עדיין נתקל בבעיה.

