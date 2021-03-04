---
title: הצג גישה מותנית של ' שלחן '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427928"
---
# <a name="monitor-intune-conditional-access"></a>הצג גישה מותנית של ' שלחן '

משתמשים המיועדים באמצעות גישה מותנית יקבלו הודעת דואר אלקטרוני אם הם אינם עומדים בדרישות הגישה של הארגון שלך. כדי לפתור, אנו ממליצים על אחד או יותר מהפתרונות הבאים:

1. אם יש להעריך את המכשיר, הקפד למשתמש לעבור לאפליקציית הפורטל של החברה ולוודא שהיא מופיעה בפורטל החברה. אם היא אינה מופיעה, על המשתמש לרשום את המכשיר.
1. בפורטל התכלת, עבור אל **כוונון**  >  **תאימות התקן**. 
1. כדי להציג את דוח תאימות המכשירים כדי לוודא שהתקן המשתמש מסומן כתואם, תחת **צג**, לחץ על **תאימות מכשיר**.
1. בפורטל התכלת, עבור אל **כוונון**  >  **תאימות התקן**. תחת **ניהול,** לחץ על **מדיניות**. ברשימת מדיניות התאימות, ודא שהפרופיל מוקצה למכשיר המשתמש שלך. אם לא הוקצה פרופיל, האפשרות ' התאמה ' לא תוכל לאשר את מצב התאימות של ההתקן.
1. ערוך את הקצאת הגישה המותנית של המשתמש.
1. בפורטל תכלת, נווט כדי **לכוונן**  >    >  **מדיניות** גישה מותנית, בחר מדיניות מתוך הרשימה ולחץ על **משתמשים וקבוצות**.
1. כדי לייעד מדיניות מסוימת לאדם כלשהו, הוסף אותם **לרשימה כלול**. כדי להבטיח שאדם מושמט מהמדיניות, הוסף אותם **לרשימת אי-הכללה**.

**קישורים שימושיים:**

- [מבט כולל על תאימות מכשירים](https://docs.microsoft.com/intune/device-compliance-get-started)
- [פתרון בעיות ב-CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [מדיניות פתרון בעיות](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [ניטור תאימות התקן של כוונון מכשיר](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> שלבים אלה שימושיים רק בפתרון בעיות בתכונה ' תכלת Active Directory ' גישה מותנית. ניתן גם להעביר הסגר על התקן שחוסם את גישת הדואר האלקטרוני שלו באמצעות מדיניות Exchange. ניתן למצוא [**כאן**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))מידע נוסף אודות ניהול מכשירים של Exchange.
