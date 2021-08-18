---
title: צג Intune מותן Access
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
ms.openlocfilehash: 2c3a382671ac95ecbaec1b374bd8c474cf9690a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327558"
---
# <a name="monitor-intune-conditional-access"></a>צג Intune מותן Access

משתמשים המתמקדים בגישה מותית יקבלו הודעת דואר אלקטרוני אם הם לא יתעדו את דרישות הגישה של הארגון שלך. כדי לפתור, מומלץ אחד או יותר מהפתרונות הבאים:

1. אם סביר להניח שהמכשיר רשום, ייעץ למשתמש לעבור לאפליקציה Company Portal ולוודא שהוא מופיע ב- Company Portal. אם לא, המשתמש חייב לרשום את המכשיר.
1. בפורטל Azure, עבור אל **תאימות התקן Intune**  >  . 
1. כדי להציג את התאימות הדוח כדי לוודא שהמכשיר של המשתמש מסומן כתואם, תחת צג , **לחץ** על **תאימות מכשירים**.
1. בפורטל Azure, עבור אל **תאימות התקן Intune**  >  . תחת **ניהול, לחץ** **על פריטי מדיניות.** ברשימת פריטי מדיניות התאימות, ודא שפרופיל מוקצה למכשיר של המשתמש שלך. אם לא הוקצה פרופיל, Intune לא יוכל לאשר את מצב התאימות של המכשיר.
1. ערוך את הקצאת הגישה המותית של המשתמש.
1. בפורטל Azure, נווט אל פריטי מדיניות גישה מותנים של **Intune**, בחר מדיניות  >    >  מהרשימה ולחץ על **משתמשים וקבוצות**.
1. כדי לייעד מדיניות מסוימת למישהו, הוסף אותו לרשימה **כלול**. כדי לוודא שאדם מושמט מהמדיניות, הוסף אותו לרשימה אל **תכלול.**

**קישורים שימושיים:**

- [מבט כולל על תאימות מכשירים](https://docs.microsoft.com/intune/device-compliance-get-started)
- [פתרון בעיות ב- CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [מדיניות פתרון בעיות](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [ניטור תאימות להתקן Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

**הערה:** שלבים אלה שימושיים רק בפתרון בעיות בתכונה Azure Active Directory תנאי Access. ניתן גם להסגר מכשיר שחוסם את גישת הדואר האלקטרוני שלו באמצעות Exchange זו. מידע נוסף על Exchange ניתן למצוא [**כאן**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).
