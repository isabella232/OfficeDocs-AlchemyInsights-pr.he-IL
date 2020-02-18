---
title: רכישת שירות עצמי של PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: 5e47e08e3309b3d58908e10ee06021da00f230bb
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091709"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="be20e-102">רכישת שירות עצמי של PowerShell</span><span class="sxs-lookup"><span data-stu-id="be20e-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="be20e-103">כדי להשתמש במודול MSCommerce PowerShell, עליך להתקין אותו בהתקן Windows 10 עם TLS 1.2 (הרשאות מנהל מקומיות הדרושות).</span><span class="sxs-lookup"><span data-stu-id="be20e-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="be20e-104">יבא והתחבר למודול MSCommerce.</span><span class="sxs-lookup"><span data-stu-id="be20e-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="be20e-105">כאשר תתבקש לבצע כניסה למערכת, יהיה עליך להשתמש באישורי תפקיד מנהל כללי או חיוב.</span><span class="sxs-lookup"><span data-stu-id="be20e-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="be20e-106">אם אין ברשותך TLS 1.2, ייתכן שתקבל את השגיאה הבאה בעת ניסיון לקבל או לעדכן את המדיניות:</span><span class="sxs-lookup"><span data-stu-id="be20e-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="be20e-107">*Errormessage-החיבור המשמש כבסיס נסגר: אירעה שגיאה לא צפויה בשליחה*.</span><span class="sxs-lookup"><span data-stu-id="be20e-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



