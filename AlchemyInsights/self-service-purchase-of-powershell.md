---
title: רכישה בשירות עצמי של PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: 48b5b0a1be1bc03d45a531a1093f18a3f750c37d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51797722"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="9ea2f-102">רכישה בשירות עצמי של PowerShell</span><span class="sxs-lookup"><span data-stu-id="9ea2f-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="9ea2f-103">כדי להשתמש במודול MSCommerce PowerShell, עליך להתקין אותו במכשיר Windows 10 עם TLS 1.2 (נדרשות הרשאות מנהל מערכת מקומיות).</span><span class="sxs-lookup"><span data-stu-id="9ea2f-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="9ea2f-104">ייבוא והתחברות למודול MSCommerce.</span><span class="sxs-lookup"><span data-stu-id="9ea2f-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="9ea2f-105">כאשר תתבקש להיכנס, יהיה עליך להשתמש באישורי תפקיד כללי או מנהל חיוב.</span><span class="sxs-lookup"><span data-stu-id="9ea2f-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="9ea2f-106">אם אין לך TLS 1.2, ייתכן שתקבל את השגיאה הבאה בעת ניסיון לקבל או לעדכן את המדיניות:</span><span class="sxs-lookup"><span data-stu-id="9ea2f-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="9ea2f-107">*ErrorMessage -החיבור שמשמש בסיס נסגר: אירעה שגיאה בלתי צפויה בשליחה.*</span><span class="sxs-lookup"><span data-stu-id="9ea2f-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



