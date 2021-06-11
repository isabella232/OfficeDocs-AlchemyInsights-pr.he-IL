---
title: שימוש באפשרויות שורת הפקודה כדי לקבוע את התצורה של הגדרות proxy Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "8024"
- "9004430"
ms.openlocfilehash: 5a25e27d7a8b128f9a60cf86a41203f8dc490216
ms.sourcegitcommit: 8878c313b41194808bd88b1f6b766f76ed17bc09
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/09/2021
ms.locfileid: "52897286"
---
# <a name="use-command-line-options-to-configure-proxy-settings-in-microsoft-edge"></a><span data-ttu-id="6f89b-102">שימוש באפשרויות שורת הפקודה כדי לקבוע את התצורה של הגדרות proxy Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="6f89b-102">Use command-line options to configure proxy settings in Microsoft Edge</span></span>

<span data-ttu-id="6f89b-103">בגירסאות Microsoft Edge 77 ואילך, מחסנית הרשת משתמשת בהגדרות הרשת של המערכת כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="6f89b-103">In Microsoft Edge versions 77 and later, the network stack uses the system's network settings by default.</span></span> <span data-ttu-id="6f89b-104">בתרחישים היברידיים שבו משתמשים מבקשים חלופה, Microsoft Edge תומך באפשרויות שורת הפקודה לקביעת תצורה של הגדרות Proxy מותאמות אישית.</span><span class="sxs-lookup"><span data-stu-id="6f89b-104">In hybrid scenarios where users request an alternative, Microsoft Edge supports command-line options for configuring custom proxy settings.</span></span> 

<span data-ttu-id="6f89b-105">לקבלת פרטים, ראה:</span><span class="sxs-lookup"><span data-stu-id="6f89b-105">For details, see:</span></span>

- [<span data-ttu-id="6f89b-106">הגדרות רשת מערכת</span><span class="sxs-lookup"><span data-stu-id="6f89b-106">System network settings</span></span>](/deployedge/edge-learnmore-cmdline-options-proxy-settings#system-network-settings)
- [<span data-ttu-id="6f89b-107">אפשרויות שורת פקודה עבור הגדרות Proxy</span><span class="sxs-lookup"><span data-stu-id="6f89b-107">Command-line options for proxy settings</span></span>](/deployedge/edge-learnmore-cmdline-options-proxy-settings#system-network-settings)
- [<span data-ttu-id="6f89b-108">הגדרות תצורה מתקדמות ואפשרויות אחרות</span><span class="sxs-lookup"><span data-stu-id="6f89b-108">Advanced configuration settings and other options</span></span>](https://go.microsoft.com/fwlink/?linkid=2134293)
- [<span data-ttu-id="6f89b-109">אופן פעולה של קבצי Cookie של Chrome SameSite</span><span class="sxs-lookup"><span data-stu-id="6f89b-109">Chrome SameSite cookie behavior</span></span>](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)