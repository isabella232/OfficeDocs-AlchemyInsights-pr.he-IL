---
title: בעיות בצירוף מחשבים אל Microsoft Defender עבור נקודות קצה
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901568"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="9aa62-102">בעיות בצירוף מחשבים אל Microsoft Defender עבור נקודות קצה</span><span class="sxs-lookup"><span data-stu-id="9aa62-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="9aa62-103">ייתכן שיש לך בעיות בצירוף מחשבים לשירות MDE.</span><span class="sxs-lookup"><span data-stu-id="9aa62-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="9aa62-104">אם אתה יכול לגשת אל מחשב משתמש הקצה, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="9aa62-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="9aa62-105">הורד את גירסת התצוגה המקדימה העדכנית ביותר של כלי האבחון של [MDE Client Analyzer](https://aka.ms/betamdeanalyzer).</span><span class="sxs-lookup"><span data-stu-id="9aa62-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="9aa62-106">לחץ באמצעות לחצן העכבר הימני על **MDEClientAnalyzer.cmd** ובחר 'הפעל כמנהל מערכת'.</span><span class="sxs-lookup"><span data-stu-id="9aa62-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="9aa62-107">פעל בהתאם להדרכה המוצעת ב- **MDEClientAnalyzer.htm**.</span><span class="sxs-lookup"><span data-stu-id="9aa62-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="9aa62-108">לקבלת יומני רישום מילוליים נוספים, סקור את תיקיית המשנה שנוצרה בשם **MDEClientAnalyzerResult**.</span><span class="sxs-lookup"><span data-stu-id="9aa62-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="9aa62-109">אם יש צורך בהדרכה נוספת, פנה אל [התמיכה של Microsoft Defender עבור נקודת קצה](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) וספק את הקובץ MDEClientAnalyzerResult.zip שנוצר לצורך ניתוח.</span><span class="sxs-lookup"><span data-stu-id="9aa62-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
