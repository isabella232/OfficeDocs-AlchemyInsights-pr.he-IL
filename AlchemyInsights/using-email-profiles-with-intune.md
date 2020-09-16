---
title: שימוש בפרופילי דואר אלקטרוני עם כוונון
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
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653289"
---
# <a name="using-email-profiles-with-intune"></a>שימוש בפרופילי דואר אלקטרוני עם כוונון

ניתן להשתמש ב-intune כדי ליצור ולפרוס פרופילי דואר אלקטרוני עבור לקוח הדואר האלקטרוני המוכלל (מוכלל) בפלטפורמות התקן מרובות.

לקבלת מידע אודות חלק מההגבלות המשויכות לפרופילי דואר אלקטרוני, כולל אופן הטיפול בנוכחות פרופילים קיימים וכיצד להסיר פרופילי דואר אלקטרוני, ראה [הוספת הגדרות דואר אלקטרוני למכשירים באמצעות ' שימוש בעידון](https://docs.microsoft.com/intune/email-settings-configure)'.

לקבלת מידע נוסף אודות אופן היצירה של פרופילי דואר אלקטרוני עבור כל פלטפורמת מכשיר, ראה:

[הגדרות התקן של Android לקביעת תצורה של דואר אלקטרוני, אימות וסינכרון בתוך המנגינה](https://docs.microsoft.com/intune/email-settings-android)  
[הוספת הגדרות דואר אלקטרוני עבור מכשירי iOS ו-iPadOS ב-Microsoft intune](https://docs.microsoft.com/intune/email-settings-ios)  
[הגדרות פרופיל דואר אלקטרוני ב-Microsoft intune עבור מכשירים שבהם פועל Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[הגדרות פרופיל דואר אלקטרוני עבור מכשירים שבהם פועל Windows 10 ב-Microsoft intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**בעיית סינכרון נפוצה**

**פרופיל הדואר האלקטרוני של נוקס ב-Android מונע מאנשי קשר, לוח שנה ומשימות של משתמשים, מלהיות מסתנכרן עם מכשירי משתמשים.**

פרופיל הדואר האלקטרוני של נוקס ב-Android נוקס מציע למנהל את האפשרות להחליט אילו סוגי תוכן מסונכרנים למכשיר על-ידי הגדרת כל אחד מהם לזמין.

אם ההגדרה עבור כל אחד מסוגי התוכן מוגדרת ל- **לא נקבעה תצורה** (ברירת המחדל), סוג תוכן זה אינו מסתנכרן באופן אוטומטי. המשתמש עשוי להפוך את סוג התוכן לזמין ישירות במכשיר באופן ידני, אך תצורה זו מוחלפת על-ידי הגדרת המדיניות ' שינוי צורה ', והסינכרון מפסיק עבור סוג תוכן זה.

