---
title: הסרת נתונים וניגוב התקנים מIntune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439649"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>הסרת נתונים וניגוב התקנים מIntune

ניתן להשתמש בפעולות מרוחקות של התקן פרישה ומחיקה של התקן כדי להסיר נתוני חברה המנוהלים על-ידי Intune או לבצע איפוס של המפעל ולהחזיר את ההתקן להגדרות ברירת המחדל שלו.

1. היכנס לניהול ההתקנים של Microsoft 365, ועבור אל **התקנים**של  >  **כל ההתקנים**.
2. בחר את ההתקן שברצונך למחוק.
3. בחר את סוג המחיקה המרוחקת שברצונך לבצע. הפרישה מוחקת רק מידע ארגוני, בעוד שמחיקות מלאות מחזירות את ההתקן להגדרות המפעל שלו.
4. בחר **כן** כדי לאשר. עד לסיום המחיקה, מצב פעולת ההתקן מוצג כממתין לפרישה.</br>
    לאחר השלמת הפעולה, לא תראה עוד את המכשיר הנייד ברשימת ההתקנים המנוהלים.

**שים לב** אין אפשרות להסיר את נתוני החברה ממכשירים המצורפים לתכלת המודעה.

לקבלת פרטים מלאים על ההשפעה של פעולות הפרישה והמחיקה, כולל מה שנשמר ומה נמחק, ראה [הסרת התקנים באמצעות ניגוב, פרישה או ביטול הרישום של ההתקן באופן ידני](https://docs.microsoft.com/intune/devices-wipe).

כדי למחוק את כל הנתונים מהתקן macOS, ראה [מחיקת כל הנתונים מהתקן macos](https://docs.microsoft.com/intune/device-erase).