---
title: קוד שגיאה 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: אם אתה מקבל שגיאה בעת הפעלת Office 2013 בפריסות של שירותים של שולחן עבודה מרוחק (RDS), שקול להפוך את ADAL לזמינה על-ידי עריכת הרישום.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709188"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="cf354-103">שגיאה בעת הפעלת Office 2013 בשירותי שולחן עבודה מרוחק</span><span class="sxs-lookup"><span data-stu-id="cf354-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="cf354-104">אם אתה מקבל שגיאה בעת הפעלת Office 2013 בפריסות של שירותים של שולחן עבודה מרוחק (RDS), שקול להפוך את ADAL לזמינה על-ידי עריכת הרישום.</span><span class="sxs-lookup"><span data-stu-id="cf354-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="cf354-105">**מפתח רישום**</span><span class="sxs-lookup"><span data-stu-id="cf354-105">**Registry key**</span></span>|<span data-ttu-id="cf354-106">**סוג**</span><span class="sxs-lookup"><span data-stu-id="cf354-106">**Type**</span></span>|<span data-ttu-id="cf354-107">**ערך**</span><span class="sxs-lookup"><span data-stu-id="cf354-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="cf354-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="cf354-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="cf354-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="cf354-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="cf354-110">1</span><span class="sxs-lookup"><span data-stu-id="cf354-110">1</span></span>  <br/> |

<span data-ttu-id="cf354-111">לקבלת מידע נוסף, ראה [הפיכת אימות מודרני לזמין עבור Office 2013 במכשירי Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="cf354-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="cf354-112">ADAL מופעל כברירת מחדל באפליקציות Microsoft 365 עבור enterprise ו-Office 2016.</span><span class="sxs-lookup"><span data-stu-id="cf354-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="cf354-113">שירותי שולחן עבודה מרוחק (RDS) נקראו בעבר ' שירותי מסופים '.</span><span class="sxs-lookup"><span data-stu-id="cf354-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  