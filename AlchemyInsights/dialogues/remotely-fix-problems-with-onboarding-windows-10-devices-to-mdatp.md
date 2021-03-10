---
title: פתרון בעיות בהפעלה מרחוק של מכשירי Windows 10 להגנת איום מתקדמת של Microsoft Defender
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693655"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>פתרון בעיות בהפעלה מרחוק של מכשירי Windows 10 להגנת איום מתקדמת של Microsoft Defender

אם באפשרותך לגשת למחשב המרוחק, בצע את הפעולות הבאות:

1. הורד את כלי האבחון של [מנתח קישוריות הלקוח](https://go.microsoft.com/fwlink/?linkid=2143466) .
2. חלץ והפעיל את MDATPAnalyzer. cmd.
3. אתר את יומן האבחון בתיקיה MDATPClientAnalyzerResult, שהיא אותה תיקיה שבה הורד את כלי המנתח.
4. כדי למצוא בעיות בקישוריות או בהגדרות של proxy באינטרנט, עיין בקובץ יומן הרישום MDATPClientAnalyzer.txt.

לקבלת מידע נוסף, ראה [בעיות במכשירים המשולבים](https://go.microsoft.com/fwlink/?linkid=2143634).
