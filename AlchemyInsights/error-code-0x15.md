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
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36526999"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="b40b7-103">אירעה שגיאה בעת הפעלת Office 2013 על שירותי שולחן עבודה מרוחק</span><span class="sxs-lookup"><span data-stu-id="b40b7-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="b40b7-104">אם אתה מקבל שגיאה בעת הפעלת Office 2013 בפריסות של שירותי שולחן עבודה מרוחק (RDS), לשקול לאפשר ADAL על-ידי עריכת הרישום.</span><span class="sxs-lookup"><span data-stu-id="b40b7-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="b40b7-105">**מפתח רישום**</span><span class="sxs-lookup"><span data-stu-id="b40b7-105">**Registry key**</span></span>|<span data-ttu-id="b40b7-106">**סוג**</span><span class="sxs-lookup"><span data-stu-id="b40b7-106">**Type**</span></span>|<span data-ttu-id="b40b7-107">**ערך**</span><span class="sxs-lookup"><span data-stu-id="b40b7-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b40b7-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="b40b7-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="b40b7-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="b40b7-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="b40b7-110">1</span><span class="sxs-lookup"><span data-stu-id="b40b7-110">1</span></span>  <br/> |

<span data-ttu-id="b40b7-111">לקבלת מידע נוסף, ראה [הפעלת אימות מודרני עבור 2013 Office בהתקני Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="b40b7-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="b40b7-112">ADAL זמינה כברירת מחדל ב- Office 365 ProPlus ו- Office 2016.</span><span class="sxs-lookup"><span data-stu-id="b40b7-112">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="b40b7-113">שירותי שולחן עבודה מרוחק (RDS) היה שם קודם לכן שירותי מסופים.</span><span class="sxs-lookup"><span data-stu-id="b40b7-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  