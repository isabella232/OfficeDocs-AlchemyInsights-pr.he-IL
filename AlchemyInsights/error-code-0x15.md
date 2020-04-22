---
title: קוד שגיאה 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: אם אתה מקבל שגיאה בעת הפעלת הפריסה של Office 2013 בפריסות של שירותי שולחן עבודה מרוחק (RDS), שקול להפוך את ADAL לזמינה על-ידי עריכת הרישום.
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703139"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="fd657-103">שגיאה בעת הפעלת Office 2013 בשירותי שולחן עבודה מרוחק</span><span class="sxs-lookup"><span data-stu-id="fd657-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="fd657-104">אם אתה מקבל שגיאה בעת הפעלת הפריסה של Office 2013 בפריסות של שירותי שולחן עבודה מרוחק (RDS), שקול להפוך את ADAL לזמינה על-ידי עריכת הרישום.</span><span class="sxs-lookup"><span data-stu-id="fd657-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="fd657-105">**מפתח רישום**</span><span class="sxs-lookup"><span data-stu-id="fd657-105">**Registry key**</span></span>|<span data-ttu-id="fd657-106">**סוג**</span><span class="sxs-lookup"><span data-stu-id="fd657-106">**Type**</span></span>|<span data-ttu-id="fd657-107">**ערך**</span><span class="sxs-lookup"><span data-stu-id="fd657-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="fd657-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="fd657-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="fd657-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="fd657-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="fd657-110">1</span><span class="sxs-lookup"><span data-stu-id="fd657-110">1</span></span>  <br/> |

<span data-ttu-id="fd657-111">לקבלת מידע נוסף, ראה [הפיכת אימות מודרני לזמין עבור Office 2013 בהתקני Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="fd657-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="fd657-112">ADAL מופעלת כברירת מחדל ב-Microsoft 365 Apps עבור הארגון ו-Office 2016.</span><span class="sxs-lookup"><span data-stu-id="fd657-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="fd657-113">שירותי שולחן עבודה מרוחק (RDS) נקראו בעבר שירותי מסופים.</span><span class="sxs-lookup"><span data-stu-id="fd657-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  