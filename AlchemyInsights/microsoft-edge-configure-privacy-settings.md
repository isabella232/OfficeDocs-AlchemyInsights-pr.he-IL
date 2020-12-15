---
title: הגדרות הפרטיות של Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677792"
---
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="fcbdd-102">הגדרות הפרטיות של Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="fcbdd-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="fcbdd-103">כברירת מחדל, אם Microsoft Edge נפרסת בפלטפורמות שאינן של Windows, נתוני אבחון ומידע אודות האתר אינם נשלחים ל-Microsoft.</span><span class="sxs-lookup"><span data-stu-id="fcbdd-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="fcbdd-104">עם זאת, אם Microsoft Edge נפרס ב-Windows 10, נתוני אבחון ומידע אודות האתר נשלחים בהתאם [להגדרות הנתונים של ' אבחון](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)משתמשים ' של Windows.</span><span class="sxs-lookup"><span data-stu-id="fcbdd-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="fcbdd-105">כדי לקבוע את האופן שבו Microsoft Edge מטפל באיסוף נתונים עבור הארגון שלך, השתמש בפריטי המדיניות הבאים של הקבוצה:</span><span class="sxs-lookup"><span data-stu-id="fcbdd-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="fcbdd-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): מדיניות זו מאפשרת דיווח על השימוש והנתונים הקשורים להתרסקות.</span><span class="sxs-lookup"><span data-stu-id="fcbdd-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="fcbdd-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): מדיניות זו שולחת מידע על האתר המשמש לשיפור שירותי Microsoft.</span><span class="sxs-lookup"><span data-stu-id="fcbdd-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="fcbdd-108">לקבלת מידע נוסף, ראה [קביעת תצורה של הגדרות מדיניות](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span><span class="sxs-lookup"><span data-stu-id="fcbdd-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>