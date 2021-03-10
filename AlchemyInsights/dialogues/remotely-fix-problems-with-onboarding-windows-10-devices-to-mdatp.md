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
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a><span data-ttu-id="b13f1-102">פתרון בעיות בהפעלה מרחוק של מכשירי Windows 10 להגנת איום מתקדמת של Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="b13f1-102">Remotely fix problems with onboarding Windows 10 devices to Microsoft Defender Advanced Threat Protection</span></span>

<span data-ttu-id="b13f1-103">אם באפשרותך לגשת למחשב המרוחק, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="b13f1-103">If you can access the remote computer, follow these steps:</span></span>

1. <span data-ttu-id="b13f1-104">הורד את כלי האבחון של [מנתח קישוריות הלקוח](https://go.microsoft.com/fwlink/?linkid=2143466) .</span><span class="sxs-lookup"><span data-stu-id="b13f1-104">Download the [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostic tool.</span></span>
2. <span data-ttu-id="b13f1-105">חלץ והפעיל את MDATPAnalyzer. cmd.</span><span class="sxs-lookup"><span data-stu-id="b13f1-105">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="b13f1-106">אתר את יומן האבחון בתיקיה MDATPClientAnalyzerResult, שהיא אותה תיקיה שבה הורד את כלי המנתח.</span><span class="sxs-lookup"><span data-stu-id="b13f1-106">Locate the diagnostic log in the MDATPClientAnalyzerResult folder, which is the same folder where the Analyzer tool was downloaded.</span></span>
4. <span data-ttu-id="b13f1-107">כדי למצוא בעיות בקישוריות או בהגדרות של proxy באינטרנט, עיין בקובץ יומן הרישום MDATPClientAnalyzer.txt.</span><span class="sxs-lookup"><span data-stu-id="b13f1-107">To find issues with connectivity or Internet proxy settings, review the log file MDATPClientAnalyzer.txt.</span></span>

<span data-ttu-id="b13f1-108">לקבלת מידע נוסף, ראה [בעיות במכשירים המשולבים](https://go.microsoft.com/fwlink/?linkid=2143634).</span><span class="sxs-lookup"><span data-stu-id="b13f1-108">To learn more, see [Issues with onboarding machines](https://go.microsoft.com/fwlink/?linkid=2143634).</span></span>
