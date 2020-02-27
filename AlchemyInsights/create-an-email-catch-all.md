---
title: ליצור דוא ל לתפוס את כל
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286194"
---
# <a name="create-an-email-catch-all"></a>ליצור דוא ל לתפוס את כל

השימוש במלכוד מאוד מיואש. מוטב לספק חזרה לשולח כדי ששולחים יידעו שההודעה שלהם לא הועברה כממוענות כדי שיוכלו לפעול. אתה יכול גם להגביל את תיבת הדואר בפיקוח לתפוס רק בעבר כתובות דוא ל חוקיים. 

כל לתפוס את כל תיבת הדואר יקבל הרבה דואר זבל והוא עשוי בסופו של דבר למלא אם לא פיקוח צמוד. (קיימים מגבלות מתקבלות.) 

אם תחליט להמשיך, בצע את הפעולות הבאות:

1. צור קבוצת תפוצה דינאמית _ אמפר _ כלול את "כל סוגי הנמענים".

2. צור תיבת דואר ייעודית לתפיסת הודעות דוא ל, לדוגמה, catchall@domain.com.

3. עבור התחום הספציפי, הגדר את הDomainType ל' ממסר הפנמה '. אם מאוחר יותר תסיר את כל המלכוד, הקפד להגדיר את התחום בחזרה לסמכותי.

4. צור כלל תעבורת דואר אלקטרוני באופן הבא:

    - אם השולח הוא "מחוץ לארגון"
    - נתב מחדש את ההודעה לCatchall@domain.com
    - אלא אם הנמען חבר ב-allusers@domain.com (קבוצת הפצה מכילה את כל החברים)
    - הקפד לאמת שתיבות דואר חדשות יתווספו לקבוצת ההפצה הדינאמית
