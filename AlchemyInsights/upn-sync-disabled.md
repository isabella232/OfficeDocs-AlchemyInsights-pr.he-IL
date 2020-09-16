---
title: סינכרון UPN אינו זמין
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749515"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="73a1c-102">סינכרון UPN אינו זמין</span><span class="sxs-lookup"><span data-stu-id="73a1c-102">UPN sync disabled</span></span>

<span data-ttu-id="73a1c-103">אם התחלת לסנכרן את התכלת לספירה לפני 30 במרץ, 2016, הפעל את ה-cmdlet הבאים של תכלת לספירה כדי להפוך התאמה רכה של UPN לזמינה עבור הארגון שלך בלבד:</span><span class="sxs-lookup"><span data-stu-id="73a1c-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="73a1c-104">**Set-MsolDirSyncFeature-EnableSoftMatchOnUpn-הפיכת התכונה לזמינה $True**</span><span class="sxs-lookup"><span data-stu-id="73a1c-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="73a1c-105">התאמה רכה של UPN מופעלת באופן אוטומטי עבור ארגונים שהתחילו לסנכרן את התכלת לספירה ב-30 במרץ או אחרי ה-30 במרץ 2016.</span><span class="sxs-lookup"><span data-stu-id="73a1c-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="73a1c-106">לקבלת מידע נוסף על הפעלת התאמה רכה ב-UPN ובתכונות סינכרון אחרות, ראה [התכונה תכלת AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="73a1c-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

