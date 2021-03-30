---
title: קביעת תצורה של הגדרות פרטיות ב- Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405107"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a><span data-ttu-id="290c0-102">קביעת תצורה של הגדרות פרטיות ב- Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="290c0-102">Configure privacy settings in Microsoft Edge</span></span>

<span data-ttu-id="290c0-103">כברירת מחדל, אם Microsoft Edge נפרס בפלטפורמות שאינן Windows, נתוני אבחון ומידע אתר אינם נשלחים ל- Microsoft.</span><span class="sxs-lookup"><span data-stu-id="290c0-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information aren't sent to Microsoft.</span></span> <span data-ttu-id="290c0-104">עם זאת, אם Microsoft Edge נפרס ב- Windows 10, נתוני אבחון ומידע אתר נשלחים בהתאם להגדרות נתוני [האבחון של Windows של המשתמשים.](https://go.microsoft.com/fwlink/?linkid=2132472)</span><span class="sxs-lookup"><span data-stu-id="290c0-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2132472).</span></span>

<span data-ttu-id="290c0-105">כדי לקבוע את התצורה של האופן שבו Microsoft Edge מטפל באיסוף נתונים עבור הארגון שלך, השתמש במדיניות הקבוצתית הבאה:</span><span class="sxs-lookup"><span data-stu-id="290c0-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="290c0-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) מפעיל דיווח על שימוש ונתונים הקשורים להתרסקות.</span><span class="sxs-lookup"><span data-stu-id="290c0-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) turns on reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="290c0-107">[SendSiteInfoToImproveServices שולח](https://go.microsoft.com/fwlink/?linkid=2132470) פרטי אתר המשמשים לשיפור שירותי Microsoft.</span><span class="sxs-lookup"><span data-stu-id="290c0-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sends site information used to improve Microsoft services.</span></span>

<span data-ttu-id="290c0-108">כדי ללמוד עוד, ראה [קביעת תצורה של הגדרות מדיניות.](https://go.microsoft.com/fwlink/?linkid=2132577)</span><span class="sxs-lookup"><span data-stu-id="290c0-108">To learn more, see [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span></span>
