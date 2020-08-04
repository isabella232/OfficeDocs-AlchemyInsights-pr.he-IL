---
title: שימוש בפרופילי דוא ל עם Intune
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
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555255"
---
# <a name="using-email-profiles-with-intune"></a>שימוש בפרופילי דוא ל עם Intune

ניתן להשתמש בIntune כדי ליצור ולפרוס פרופילי דואר אלקטרוני עבור לקוח הדואר האלקטרוני יליד (מובנה) בפלטפורמות התקן מרובות.

לקבלת מידע אודות חלק מההגבלות המשויכות לפרופילי דואר אלקטרוני, כולל אופן הטיפול בפרופילים קיימים וכיצד להסיר פרופילי דואר אלקטרוני, ראה [הוספת הגדרות דואר אלקטרוני להתקנים באמצעות Intune](https://docs.microsoft.com/intune/email-settings-configure).

לקבלת מידע נוסף על אופן יצירת פרופילי דואר אלקטרוני עבור כל פלטפורמת התקן, ראה:

[הגדרות התקן אנדרואיד כדי לקבוע תצורה של דואר אלקטרוני, אימות וסנכרון בIntune](https://docs.microsoft.com/intune/email-settings-android)  
[הוספת הגדרות דואר אלקטרוני עבור iOS והתקני iPadOS ב-Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[הגדרות פרופיל דואר אלקטרוני ב-Microsoft Intune עבור התקנים המפעילים את Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[הגדרות פרופיל דואר אלקטרוני עבור התקנים שבהם פועל Windows 10 ב-Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**בעיית סינכרון משותפת**

**נוקס על פרופיל דוא ל אנדרואיד מונע משתמשים אנשי קשר, לוח שנה, ומשימות, מלהיות מסונכרן להתקני משתמש.**

נוקס על דמוי אדם נוקס פרופיל דוא ל מציע למנהל את האפשרות להחליט אילו סוגי תוכן מסונכרנים למכשיר על ידי הגדרת כל אחד מאופשר.

אם ההגדרה עבור אחד מסוגי התוכן מוגדרת **כ'לא נקבעה** ' (ברירת המחדל), סוג תוכן זה אינו מסונכרן באופן אוטומטי. משתמש עשוי לאפשר את סוג התוכן הרצוי ישירות על ההתקן באופן ידני, אך תצורה זו מוחלפת בהגדרת המדיניות Intune והסינכרון נפסק עבור סוג תוכן זה.

