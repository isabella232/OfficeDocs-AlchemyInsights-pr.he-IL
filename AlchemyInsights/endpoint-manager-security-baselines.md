---
title: EndPoint Manager - תוכניות בסיסיות של אבטחה
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51420880"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager - תוכניות בסיסיות של אבטחה

תוכניות בסיסיות אבטחה הן קבוצות מוגדרות מראש של הגדרות Windows, שיעזור לך להחיל את הגדרות האבטחה המומלצות על-ידי צוותי האבטחה הרלוונטיים. ניתן להתאים אישית תוכניות בסיסיות אלה כדי לספק רק את ההגדרות והערכים הרצויים. לקבלת מידע נוסף אודות תוכניות בסיסיות של אבטחה, ראה [שימוש בתוכנית בסיסית של אבטחה כדי לקבוע את התצורה של מכשירי Windows 10 ב- Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

כיום זמינים תוכניות בסיסיות עבור מוצרים אלה:

- הגדרות אבטחה של Windows MDM
- Microsoft Defender עבור אבטחת EndPoint
- מייקרוסופט אדג'

כל אחת מ בסיסית מתעדכנת מעת לעת ומופץ בגירסאות מצטברות. כל גירסה מוסיפה או מסירה הגדרות מהגירסה הקודמת כדי להבטיח שה בסיסית תיפגש עם ההנחיות הנוכחיות. מסוף תוכניות בסיסיות של אבטחה באבטחת נקודות קצה מאפשר השוואה בין גירסאות שונות על-ידי הפיכת השינויים מגירסה לגירסה לגלויים.

לקבלת הדרכה כיצד לשנות בצורה היעילה ביותר את גירסת התוכנית הבסיסית שנפרסת, ראה [ניהול פרופילי תוכנית בסיסית של אבטחה ב- Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

לאחר פריסת תוכנית בסיסית של אבטחה, באפשרותך לנטר את מצב הפריסה וביקורות ההגדרות על בסיס מכשיר אחר מכשיר.

**הערה:** נתוני הדיווח עבור תוכניות בסיסיות עשויים להתקדם עד 24 שעות מהפריסה הראשונית למכשיר ועד 6 שעות לעדכונים נוספים. 

הסיבה הנפוצה ביותר להגדרה בסיסית אינה חלה היא משום שהגדרה זו נמצאת בשימוש בפרופיל אחר. ניתן לחקור תרחיש זה עבור מכשיר ספציפי על-ידי בחירת מכשיר זה מתוך הצומת מצב התקן של פרופיל 'תוכנית בסיסית של אבטחה'. לקבלת פרטים, ראה [פתרון התנגשויות עבור תוכניות בסיסיות של אבטחה.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)