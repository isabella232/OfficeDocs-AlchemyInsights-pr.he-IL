---
title: סינכרון UPN זמין
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: d00f10688ec775c22d60a9089e291c265ada46f1
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28292863"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="f91b6-102">סינכרון UPN זמין</span><span class="sxs-lookup"><span data-stu-id="f91b6-102">UPN sync disabled</span></span>

<span data-ttu-id="f91b6-103">אם התחלת סינכרון AD תכלת הרקיע לפני ה-30 במרץ, 2016, כדי להפעיל cmdlet AD PowerShell תכלת הרקיע הבאות כדי לאפשר התאמה רכים UPN עבור הארגון שלך בלבד:</span><span class="sxs-lookup"><span data-stu-id="f91b6-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="f91b6-104">**ערכת-MsolDirSyncFeature-תכונה EnableSoftMatchOnUpn-אפשר $True**</span><span class="sxs-lookup"><span data-stu-id="f91b6-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="f91b6-105">התאמת רכים UPN מופעלת באופן אוטומטי עבור ארגונים שהפעילה לסנכרן AD תכלת הרקיע או לאחר 30 במרץ, 2016.</span><span class="sxs-lookup"><span data-stu-id="f91b6-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="f91b6-106">לקבלת מידע נוסף אודות הפיכת התאמה רכים UPN ותכונות אחרות של סינכרון, נא עיין [התחבר AD תכלת הרקיע התכונות של שירות הסינכרון](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="f91b6-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

