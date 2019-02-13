---
title: AADConnect שדרוג 932
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8038d5ef768d6ee228db7d038ad71d926f4047f3
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29937945"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="49c2d-102">שדרוג AD תכלת הרקיע להתחבר</span><span class="sxs-lookup"><span data-stu-id="49c2d-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="49c2d-p101">כברירת מחדל, שדרוג אוטומטי זמין עבור התחברות AD תכלת הרקיע, המסייעת להבטיח לך אתה מפעיל את הגירסה העדכנית ביותר. כדי לוודא את הגדרות השדרוג האוטומטי, השתמש cmdlet **Get-ADSyncAutoUpgrade** ב- AD PowerShell תכלת הרקיע. ה-cmdlet תחזיר את אחד הערכים הבאים:</span><span class="sxs-lookup"><span data-stu-id="49c2d-p101">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version. To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell. The cmdlet will return one of following values:</span></span> 
  
- <span data-ttu-id="49c2d-106">**זמין**: שדרוג אוטומטי מופעלת.</span><span class="sxs-lookup"><span data-stu-id="49c2d-106">**Enabled**: Automatic upgrade is enabled.</span></span> 
    
- <span data-ttu-id="49c2d-107">**זמין**: שדרוג אוטומטי אינו זמין.</span><span class="sxs-lookup"><span data-stu-id="49c2d-107">**Disabled**: Automatic upgrade is disabled.</span></span> 
    
- <span data-ttu-id="49c2d-p102">**מושעה**: המערכת כבר לא זכאי לקבל שדרוגים אוטומטיים. אין באפשרותך להגדיר ערך זה; הוא מוגדר על-ידי המערכת.</span><span class="sxs-lookup"><span data-stu-id="49c2d-p102">**Suspended**: The system is no longer eligible to receive automatic upgrades. You can't configure this value; it's set by the system.</span></span> 
    
<span data-ttu-id="49c2d-110">לקבלת מידע נוסף, ראה [שדרוג אוטומטי](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="49c2d-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>
  
<span data-ttu-id="49c2d-111">כדי להוריד את הגירסה העדכנית ביותר של חיבור AD תכלת הרקיע, עבור אל [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="49c2d-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
  

