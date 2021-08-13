---
title: שימוש בפרופילי דואר אלקטרוני עם Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: b1653b73e7296e7eed411ae73c19342a1187b2eb7e287cff4339ea0ca32d75c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919424"
---
# <a name="using-email-profiles-with-intune"></a>שימוש בפרופילי דואר אלקטרוני עם Intune

Intune יכול לשמש ליצירה ולפריסה של פרופילי דואר אלקטרוני עבור לקוח הדואר האלקטרוני המקורי (המוכלל) בפלטפורמות מכשירים מרובות.

לקבלת מידע אודות חלק מההגבלות המשויכות לפרופילי דואר אלקטרוני, כולל האופן בו הנוכחות של פרופילים קיימים מטופלת ואופן הסרת פרופילי דואר אלקטרוני, ראה הוספת [הגדרות דואר אלקטרוני למכשירים באמצעות Intune](https://docs.microsoft.com/intune/email-settings-configure).

לקבלת מידע נוסף אודות יצירת פרופילי דואר אלקטרוני עבור כל פלטפורמת מכשיר, ראה:

[הגדרות מכשיר Android לקביעת התצורה של דואר אלקטרוני, אימות וסינכרון ב- Intune](https://docs.microsoft.com/intune/email-settings-android)  
[הוספת הגדרות דואר אלקטרוני עבור מכשירי iOS ו- iPadOS ב- Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[הגדרות פרופיל דואר אלקטרוני ב- Microsoft Intune עבור מכשירים פועלים Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[הגדרות פרופיל דואר אלקטרוני עבור מכשירים Windows 10 ב- Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**בעיית סינכרון נפוצה**

**פרופיל דואר אלקטרוני של KNOX ב- Android מונע סינכרון של אנשי קשר, לוח שנה ומשימות של משתמש למכשירי משתמש.**

פרופיל הדואר האלקטרוני של KNOX ב- Android KNOX מציע למנהל המערכת אפשרות להחליט אילו סוגי תוכן מסתנכרנים למכשיר על-ידי הגדרת כל אחד מהם לזמין.

אם ההגדרה עבור אחד מסוגי  התוכן מוגדרת כ'לא מוגדר' (ברירת המחדל), סוג תוכן זה אינו מסתנכרן באופן אוטומטי. משתמש עשוי להפוך את סוג התוכן הרצוי לזמין ישירות במכשיר באופן ידני, אך תצורה זו מוחלפת על-ידי הגדרת המדיניות Intune, והסינכרון מפסיק עבור סוג תוכן זה.

