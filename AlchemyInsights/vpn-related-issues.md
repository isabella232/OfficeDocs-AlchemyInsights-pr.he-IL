---
title: בעיות הקשורות ל-VPN
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555237"
---
# <a name="vpn-related-issues"></a>בעיות הקשורות ל-VPN

יישום מוצלח של קישוריות VPN עבור לקוחות MDM תלוי בפרופיל שנפרס המשקף בצורה נכונה את הדרישות של תשתית ה-VPN. לקבלת ההגדרות המתאימות עבור פלטפורמות הלקוח שאתה חוקר, ראה: 

[Windows 10 והגדרות התקן הולוגרפית של Windows כדי להוסיף חיבורי VPN באמצעות Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[הוסף הגדרות VPN על iOS ו-iPadOS התקנים ב-Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[הגדרות אנדרואיד התקן להגדיר VPN ב Intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[הוסף הגדרות VPN על התקני macOS ב-Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

אם פרופיל ה-VPN משתמש באימות המבוסס על אישורים, ודא שאישור הבסיס ופרופילי אישורי אימות הלקוח המקושרים לפרופיל ה-VPN נפרסים בהצלחה.

**סוגיות נפוצות**

**הפרסתי פרופיל VPN למכשיר. Intune מראה כי זה היה מוצלח, אבל המכשיר אינו מתחבר ל-VPN.**

מצב מוצלח פירושו שIntune בהצלחה את הפרופיל כפי שהוגדר. עם זאת, ייתכן שתצורות אלה לא יתאימו לדרישות הרשת ו/או האימות שלך. סקירת יומני רישום בשירות התשתית והאימות (בשרת VPN ובשרת NPS/Radius) לקבלת פרטים נוספים אודות ניסיון החיבור. ייתכן שתצטרך לעבוד עם צוות תשתית הרשת, או ספק ה-VPN של ספק חיצוני, כדי לאסוף ולסקור יומני רישום.

**כאשר אני מגדיר VPN מותאם אישית עבור iOS, התכונה per-app VPN לא נעשה זמין.**

Per-app VPN עבור מכשירי iOS ב Intune זמין כעת רשימה מסוימת של ספקים ושותפים, מי חייב גם לעמוד בדרישות המוקדמות אישור לפני הגדרת VPN לפי app. לקבלת מידע נוסף, ראה [הגדרת לכל יישום רשת פרטית וירטואלית (VPN) עבור iOS/iPadOS התקנים ב Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

לקבלת מידע נוסף על כל סוגי החיבור VPN ב Intune, ראה [יצירת פרופילי vpn כדי להתחבר שרתי vpn ב Intune](https://docs.microsoft.com/intune/vpn-settings-configure).  

**iOS On-דרישה VPN אינו מפעיל כאשר הגישה לתחום שתצורתו נקבעה**

כדי לבדוק את הגדרות ה-VPN האוטומטיות, הגדר את הערכים הבאים:

ברצוני לבצע את הפעולות הבאות: **הערכת כל ניסיון לחיבור** 

בחר אם להתחבר: **התחבר במידת הצורך**

כאשר משתמשים ניגשים לתחומים אלה: *שם תחום* **יעד**

אם התצורה שלעיל אינה מוצלחת, הוסף את הרכיב הבא:

כאשר כתובת URL זו אינה נגישה, הכוח לחבר את ה-VPN: **Badurl**