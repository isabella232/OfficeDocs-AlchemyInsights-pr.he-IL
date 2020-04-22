---
title: סינכרון UPN לא זמין
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 33bc7e30d41ff70e2ce55d946202acf45dbcb0f2
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726105"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="f2aa3-102">סינכרון UPN לא זמין</span><span class="sxs-lookup"><span data-stu-id="f2aa3-102">UPN sync disabled</span></span>

<span data-ttu-id="f2aa3-103">אם התחלתם לסנכרן לפני התכלת לפני 30 במרץ 2016, הפעל את ה-cmdlet הבאים של תכלת לספירה כדי לאפשר התאמה של UPN רך לארגון שלך בלבד:</span><span class="sxs-lookup"><span data-stu-id="f2aa3-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="f2aa3-104">**Set-מחיילים מערכת התכונות-הפוך לזמין $True**</span><span class="sxs-lookup"><span data-stu-id="f2aa3-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="f2aa3-105">התאמה ל-UPN רכה מופעלת באופן אוטומטי עבור ארגונים שהחלו לסנכרן לתכלת AD ב-30 במרץ, 2016.</span><span class="sxs-lookup"><span data-stu-id="f2aa3-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="f2aa3-106">כדי ללמוד עוד אודות הפעלת התאמה רכה ב-UPN ובתכונות סינכרון אחרות, נא עיין [בתכונות שירות הסינכרון של התכלת](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="f2aa3-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

