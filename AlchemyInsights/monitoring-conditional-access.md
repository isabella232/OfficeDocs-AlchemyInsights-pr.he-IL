---
title: ניטור גישה מותנית
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366429"
---
# <a name="monitoring-conditional-access-for-exchange"></a>ניטור הגישה המותנית עבור Exchange

משתמשים המיועדים באמצעות גישה מותנית יקבלו הודעת דואר אלקטרוני אם הם אינם עומדים בדרישות הגישה של הארגון שלך. כדי לפתור, אנו ממליצים על אחד או יותר מהפתרונות הבאים:

- אם יש להעריך את המכשיר, הקפד למשתמש לעבור לאפליקציית הפורטל של החברה ולוודא שהיא מופיעה בפורטל החברה. אם היא אינה מופיעה, המשתמש צריך לרשום את המכשיר.
- בפורטל התכלת, עבור אל כוונון תאימות התקן >. תחת צג, לחץ על תאימות מכשיר. הצג את דוח תאימות המכשירים כדי לוודא שהתקן המשתמש מסומן כתואם.
- בפורטל התכלת, עבור אל כוונון תאימות התקן >. תחת ניהול, לחץ על מדיניות. ברשימת מדיניות התאימות, ודא שהפרופיל מוקצה למכשיר המשתמש שלך. אם לא הוקצה פרופיל, האפשרות ' התאמה ' לא תוכל לאשר את מצב התאימות של ההתקן.
- ערוך את הקצאת הגישה המותנית של המשתמש.

1. בפורטל ' תכלת ', עבור אל ' **שלחן**  >  **Conditional access**  >  **מדיניות**גישה מותנית '.
2. בחר מדיניות מהרשימה.
3. לחץ על משתמשים וקבוצות.
4. כדי לייעד מדיניות מסוימת לאדם כלשהו, הוסף אותם לרשימה כלול. כדי להבטיח שאדם מושמט מהמדיניות, הוסף אותם לרשימת אי-הכללה.

קישורים שימושיים:

[מבט כולל על תאימות מכשירים](https://docs.microsoft.com/intune/device-compliance-get-started)

[פתרון בעיות ב-CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[מדיניות פתרון בעיות](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[ניטור תאימות התקן של כוונון מכשיר](https://docs.microsoft.com/intune/compliance-policy-monitor)

הערה: שלבים אלה שימושיים רק בפתרון בעיות בתכונה ' תכלת Active Directory ' גישה מותנית. ניתן גם להעביר הסגר על התקן שחוסם את גישת הדואר האלקטרוני שלו באמצעות מדיניות Exchange. ניתן למצוא [כאן](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>)מידע נוסף אודות ניהול מכשירים של Exchange.
