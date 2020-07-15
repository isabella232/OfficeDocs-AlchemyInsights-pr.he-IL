---
title: בעיות במכונות העלייה למטוס
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141468"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="10053-102">בעיות במכונות העלייה למטוס</span><span class="sxs-lookup"><span data-stu-id="10053-102">Issues with onboarding machines</span></span>

<span data-ttu-id="10053-103">ייתכן שיהיו לך בעיות עם מכונות העלייה למטוס לשירות MDATP.</span><span class="sxs-lookup"><span data-stu-id="10053-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="10053-104">אם באפשרותך לגשת למחשב משתמש הקצה, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="10053-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="10053-105">הורד את כלי האבחון של [מנתח הקישוריות של הלקוח](https://aka.ms/mdatpanalyzer) .</span><span class="sxs-lookup"><span data-stu-id="10053-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="10053-106">חלץ והפעל את MDATPAnalyzer. cmd.</span><span class="sxs-lookup"><span data-stu-id="10053-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="10053-107">אתר את יומן האבחון בתיקיה שנקראת Mdatpלקוחוהתוצאת המערכת, אותה תיקיה שבה מתבצעת הורדה של כלי המנתח.</span><span class="sxs-lookup"><span data-stu-id="10053-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="10053-108">סקור את קובץ יומן הרישום, MDATPClientAnalyzer.txt כדי למצוא בעיות קישוריות או הגדרות proxy באינטרנט.</span><span class="sxs-lookup"><span data-stu-id="10053-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>