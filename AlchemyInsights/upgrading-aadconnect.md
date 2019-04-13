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
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8ffa8f64019077034bc4fad61d1d843849c42898
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/13/2019
ms.locfileid: "31858961"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="0120e-102">שדרוג AD תכלת הרקיע להתחבר</span><span class="sxs-lookup"><span data-stu-id="0120e-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="0120e-103">כברירת מחדל, שדרוג אוטומטי זמין עבור התחברות AD תכלת הרקיע, המסייעת להבטיח לך אתה מפעיל את הגירסה העדכנית ביותר.</span><span class="sxs-lookup"><span data-stu-id="0120e-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="0120e-104">כדי לוודא את הגדרות השדרוג האוטומטי, השתמש cmdlet **Get-ADSyncAutoUpgrade** ב- AD PowerShell תכלת הרקיע.</span><span class="sxs-lookup"><span data-stu-id="0120e-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="0120e-105">ה-cmdlet תחזיר את אחד הערכים הבאים:</span><span class="sxs-lookup"><span data-stu-id="0120e-105">The cmdlet will return one of following values:</span></span> 

- <span data-ttu-id="0120e-106">**זמין**: שדרוג אוטומטי מופעלת.</span><span class="sxs-lookup"><span data-stu-id="0120e-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="0120e-107">**זמין**: שדרוג אוטומטי אינו זמין.</span><span class="sxs-lookup"><span data-stu-id="0120e-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="0120e-108">**מושעה**: המערכת כבר לא זכאי לקבל שדרוגים אוטומטיים.</span><span class="sxs-lookup"><span data-stu-id="0120e-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="0120e-109">אין באפשרותך להגדיר ערך זה; הוא מוגדר על-ידי המערכת.</span><span class="sxs-lookup"><span data-stu-id="0120e-109">You can't configure this value; it's set by the system.</span></span> 

<span data-ttu-id="0120e-110">לקבלת מידע נוסף, ראה [שדרוג אוטומטי](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="0120e-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="0120e-111">כדי להוריד את הגירסה העדכנית ביותר של חיבור AD תכלת הרקיע, עבור אל [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="0120e-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
