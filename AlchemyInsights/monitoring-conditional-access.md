---
title: ניטור מותן Access
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
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975102"
---
# <a name="monitoring-conditional-access-for-exchange"></a>ניטור Access מותן Exchange

משתמשים המתמקדים בגישה מותית יקבלו הודעת דואר אלקטרוני אם הם לא יתעדו את דרישות הגישה של הארגון שלך. כדי לפתור, מומלץ אחד או יותר מהפתרונות הבאים:

- אם סביר להניח שהמכשיר רשום, ייעץ למשתמש לעבור לאפליקציה Company Portal ולוודא שהוא מופיע ב- Company Portal. אם לא, המשתמש צריך לרשום את המכשיר.
- בפורטל Azure, עבור אל Intune > התקן. תחת צג, לחץ על תאימות להתקן. הצג את התאימות הדוח כדי לוודא שהמכשיר של המשתמש מסומן כתואם.
- בפורטל Azure, עבור אל Intune > התקן. תחת ניהול, לחץ על פריטי מדיניות. ברשימת פריטי מדיניות התאימות, ודא שפרופיל מוקצה למכשיר של המשתמש שלך. אם לא הוקצה פרופיל, Intune לא יוכל לאשר את מצב התאימות של המכשיר.
- ערוך את הקצאת הגישה המותית של המשתמש.

1. בפורטל Azure, עבור אל **פריטי מדיניות גישה**  >  **מותנים של** Intune  >  .
2. בחר מדיניות מהרשימה.
3. לחץ על משתמשים וקבוצות.
4. כדי לייעד מדיניות מסוימת למישהו, הוסף אותו לרשימה כלול. כדי לוודא שאדם מושמט מהמדיניות, הוסף אותו לרשימה אל תכלול.

קישורים שימושיים:

[מבט כולל על תאימות מכשירים](https://docs.microsoft.com/intune/device-compliance-get-started)

[פתרון בעיות ב- CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[מדיניות פתרון בעיות](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[ניטור תאימות למכשיר Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

הערה: שלבים אלה שימושיים רק בפתרון בעיות בתכונה Azure Active Directory תנאי Access. ניתן גם להסגר מכשיר שחוסם את גישת הדואר האלקטרוני שלו באמצעות Exchange המדיניות. מידע נוסף על Exchange ניתן למצוא את ניהול המכשירים [כאן]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
