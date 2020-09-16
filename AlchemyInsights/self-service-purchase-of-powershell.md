---
title: רכישה בשירות עצמי של PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: e6cc504ebef19cbe78f576d9b207fe2d951d0ef5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47739971"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="e7fdd-102">רכישה בשירות עצמי של PowerShell</span><span class="sxs-lookup"><span data-stu-id="e7fdd-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="e7fdd-103">כדי להשתמש במודול MSCommerce PowerShell, עליך להתקין אותו במכשיר Windows 10 עם TLS 1.2 (נדרשת הרשאות מנהל מערכת מקומי).</span><span class="sxs-lookup"><span data-stu-id="e7fdd-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="e7fdd-104">יבא והתחבר למודול MSCommerce.</span><span class="sxs-lookup"><span data-stu-id="e7fdd-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="e7fdd-105">כאשר תתבקש להיכנס, יהיה עליך להשתמש באישורי תפקיד של מנהל מערכת כללי או חיוב.</span><span class="sxs-lookup"><span data-stu-id="e7fdd-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="e7fdd-106">אם אין ברשותך TLS 1.2, ייתכן שתקבל את השגיאה הבאה בעת ניסיון לקבל או לעדכן את המדיניות:</span><span class="sxs-lookup"><span data-stu-id="e7fdd-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="e7fdd-107">*ErrorMessage-החיבור המשמש כבסיס נסגר: אירעה שגיאה בלתי צפויה בשליחה*.</span><span class="sxs-lookup"><span data-stu-id="e7fdd-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



