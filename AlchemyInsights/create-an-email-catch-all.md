---
title: יצירת הודעת דואר אלקטרוני לתפוס את כל
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712987"
---
# <a name="create-an-email-catch-all"></a>יצירת הודעת דואר אלקטרוני לתפוס את כל

השימוש במלכוד כולו מבוטל מאוד. מוטב לספק חזרה לשולח המאפשר לשולחים לדעת שאין אפשרות לשלוח את ההודעה שלהם ככתובת, כדי שיוכלו לפעול. באפשרותך גם להגביל את תיבת הדואר המנוטר כדי ללכוד רק כתובות דואר אלקטרוני חוקיות בעבר. 

כל תיבת דואר של כל מציאה תקבל הודעת דואר זבל מצויינת וייתכן שתתמלא בסופו של דבר אם לא יתבצע פיקוח מקרוב. (קיימות מגבלות מתקבלות.) 

אם תחליט להמשיך, בצע את הפעולות הבאות:

1. יצירת קבוצת תפוצה דינאמית & כלול את כל סוגי הנמענים.

2. צור תיבת דואר ייעודית כדי לתפוס הודעות דואר אלקטרוני, לדוגמה, catchall@domain.com.

3. עבור התחום הספציפי, הגדר את DomainType "InternalRelay". אם לאחר מכן תסיר את האפשרות תפוס הכל, הקפד להגדיר את התחום בחזרה לסמכותי.

4. צור כלל תעבורה של זרימת דואר באופן הבא:

    - אם השולח הוא "מחוץ לארגון"
    - ניתוב מחדש של ההודעה ל-Catchall@domain.com
    - למעט אם הנמען הוא חבר ב-allusers@domain.com (קבוצת תפוצה מכילה את כל החברים)
    - הקפד לוודא שתיבות דואר חדשות נוספות לקבוצת התפוצה הדינאמית
