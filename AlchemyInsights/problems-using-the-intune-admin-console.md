---
title: בעיות בשימוש במסוף הניהול של Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555382"
---
# <a name="problems-using-the-intune-admin-console"></a>בעיות בשימוש במסוף הניהול של Intune

**"הגישה נדחתה" בעת ניווט בפורטל הניהול של Intune.**

- אם אתה חבר בתפקיד מותאם אישית Intune, ודא שרשיון של Intune או ' חבילת ניידות ארגונית ' (EMS) מוקצה לחשבונך.
- אם אתה משתמש ב'מנהל התצורה ' כדי לנהל התקנים, ודא שאינך חלק מאוסף המשתמשים Intune עבור מנהל התצורה MDM.
- ודא שהוקצתה לך הרשאות בקרת ניהול מבוססת תפקידים (RBAC) המתאימות בלהב התפקידים Intune.
- ודא שהקבוצה שבשימוש אינה רשימת תפוצה. Intune בפורטל התכלת תומך רק בחשבונות משתמשים השייכים לקבוצות האבטחה של הפעילות התכלת של הספרייה. סקור את הקבוצות שלך בפורטל התכלת **הIntune**  >  **קבוצות**, או בפורטל **הפעיל של הספרייה הפעילה**.

**למשתמש יש הרשאות רבות מדי עבור תפקיד Intune שהוקצה**

ייעץ למשתמש לעבור אל **Intune**  >  **Intune תפקידים**  >  **שההרשאות שלי**  >  **מייצאים** כדי לסקור הרשאות מוענקות.

**הוספתי קבוצת טווחים לתפקיד, אך משתמשים באותו תפקיד עדיין יראו משתמשים או התקנים אחרים.**

קבוצות טווחים אינן מסננות משתמשים או התקנים. קבוצות טווחים:

- הגבלה למי משתמשים יכולים להקצות מדיניות או יישומים.
- אפשר למשתמשים מסוימים בלבד להפעיל משימות מרוחקות בהתקנים.

לקבלת מידע נוסף אודות קבוצות היקף, ראה [בקרת גישה מבוססת תפקידים (RBAC) עם Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**הוספתי משתמש לתפקיד Intune אך עדיין יש להם גישה מלאה למסוף הניהול של Intune.**

נווט אל Intune > **משתמשים** בפורטל התכלת וודא שהמשתמש אינו מוקצה לאף אחד מהתפקידים הבאים בפורטל התכלת:

- מנהל מערכת כללי
- מנהל שירות Intune
- מנהל מערכת של SharePoint

לקבלת מידע נוסף, ראה [בקרת גישה מבוססת תפקידים (RBAC) עם Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**בעיות גישה**

לקבלת מידע נוסף, ראה [אינך יכול להיכנס ל-Office 365, תכלת או Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).