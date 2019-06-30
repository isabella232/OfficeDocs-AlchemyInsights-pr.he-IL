---
title: קוד שגיאה 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: אם אתה מקבל שגיאה בעת הפעלת Office 2013 בפריסות של שירותי שולחן עבודה מרוחק (RDS), לשקול לאפשר ADAL על-ידי עריכת הרישום.
ms.openlocfilehash: e2249d8ebbd2313c64dda5656a3243fa76d97a9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35388246"
---
<span data-ttu-id="abd70-103">אם אתה מקבל שגיאה בעת הפעלת Office 2013 בפריסות של שירותי שולחן עבודה מרוחק (RDS), לשקול לאפשר ADAL על-ידי עריכת הרישום.</span><span class="sxs-lookup"><span data-stu-id="abd70-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="abd70-104">**מפתח רישום**</span><span class="sxs-lookup"><span data-stu-id="abd70-104">**Registry key**</span></span>|<span data-ttu-id="abd70-105">**סוג**</span><span class="sxs-lookup"><span data-stu-id="abd70-105">**Type**</span></span>|<span data-ttu-id="abd70-106">**ערך**</span><span class="sxs-lookup"><span data-stu-id="abd70-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="abd70-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="abd70-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="abd70-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="abd70-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="abd70-109">1</span><span class="sxs-lookup"><span data-stu-id="abd70-109">1</span></span>  <br/> |

<span data-ttu-id="abd70-110">לקבלת מידע נוסף, ראה [הפעלת אימות מודרני עבור 2013 Office בהתקני Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="abd70-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="abd70-111">ADAL זמינה כברירת מחדל ב- Office 365 ProPlus ו- Office 2016.</span><span class="sxs-lookup"><span data-stu-id="abd70-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="abd70-112">> שירותי שולחן עבודה מרוחק (RDS) היה שם קודם לכן שירותי מסופים.</span><span class="sxs-lookup"><span data-stu-id="abd70-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  