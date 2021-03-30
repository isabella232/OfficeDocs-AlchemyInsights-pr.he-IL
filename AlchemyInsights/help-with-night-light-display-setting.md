---
title: עזרה בהגדרת תצוגת אור הלילה
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404662"
---
# <a name="help-with-the-night-light-display-setting"></a>עזרה בהגדרת תצוגת אור הלילה

לקבלת מידע נוסף על הגדרות התצוגה של שעות הלילה, ראה [הגדרת התצוגה שלך לזמן לילה ב- Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).

אם אפשרויות אור הלילה מופיעות באפור בהגדרות, בדוק את מנהל התצוגה: 

1. לחץ על תיבת החיפוש בשורת המשימות והקלד **מנהל ההתקנים** ולאחר מכן בחר **מנהל ההתקנים** בתוצאות החיפוש.
1. הרחב **את מתאמי תצוגה**. 

למרבה הצער, תכונת אור הלילה אינה זמינה אם המכשיר שלך משתמש במנהל התקן DisplayLink או במנהל התקן תצוגה בסיסי.

תכונת אור הלילה משתמשת בטכנולוגיית הגרפיקה האחרונה, כך שייתכן שתצטרך לעדכן את מנהל התצוגה:  

- בדוק אם קיימים עדכונים **על-ידי עבור אל** התחל  >  **הגדרות** עדכון &  >  **אבטחה** Windows  >  **Update בדוק** אם  >  **קיימים עדכונים.**  

או

- בקר באתר האינטרנט של התמיכה של יצרן החומרה כדי להוריד ולהתקין באופן ידני את מנהלי ההתקנים העדכניים ביותר של התצוגה.

## <a name="reset-night-light-in-the-registry"></a>איפוס אור לילה ברישום

אם עדכון מנהל התצוגה לא עבד, ייתכן שתצטרך לאפס את אור הלילה ברישום.  

**שים לב:** שלב פתרון בעיות זה מומלץ רק עבור משתמשים מתקדמים. בעיות חמורות עלולות להתרחש אם תשנה את הרישום באופן שגוי. לקבלת הגנה נוספת, גבה את הרישום לפני שינויו כדי שתוכל לשחזר אותו אם מתרחשות בעיות.

1. בתיבת החיפוש, הקלד **regedit** ולאחר מכן בחר **עורך הרישום** בתוצאות החיפוש.

1. עבור אל מפתח הרישום הבא: 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. יצא ולאחר מכן מחק את מפתח המשנה הבא:$$windows.data.bluelightreduction.bluelightreductionstate

1. יצא ולאחר מכן מחק את מפתח המשנה הבא:$$windows.data.bluelightreduction.settings

1. הפעל מחדש את Windows וודא אם האפשרויות של אור הלילה זמינות.


