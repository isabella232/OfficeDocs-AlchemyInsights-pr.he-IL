---
title: AADConnect שדרוג 932
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: ff3f74348599788edd8ce0991fe49bb6a54b55af
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506084"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="5697e-102">שדרוג AD תכלת הרקיע להתחבר</span><span class="sxs-lookup"><span data-stu-id="5697e-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="5697e-103">כברירת מחדל, שדרוג אוטומטי זמין עבור התחברות AD תכלת הרקיע, המסייעת להבטיח לך אתה מפעיל את הגירסה העדכנית ביותר.</span><span class="sxs-lookup"><span data-stu-id="5697e-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="5697e-104">כדי לוודא את הגדרות השדרוג האוטומטי, השתמש cmdlet **Get-ADSyncAutoUpgrade** ב- AD PowerShell תכלת הרקיע.</span><span class="sxs-lookup"><span data-stu-id="5697e-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="5697e-105">ה-cmdlet תחזיר את אחד הערכים הבאים:</span><span class="sxs-lookup"><span data-stu-id="5697e-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="5697e-106">**זמין**: שדרוג אוטומטי מופעלת.</span><span class="sxs-lookup"><span data-stu-id="5697e-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="5697e-107">**זמין**: שדרוג אוטומטי אינו זמין.</span><span class="sxs-lookup"><span data-stu-id="5697e-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="5697e-108">**מושעה**: המערכת כבר לא זכאי לקבל שדרוגים אוטומטיים.</span><span class="sxs-lookup"><span data-stu-id="5697e-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="5697e-109">אין באפשרותך להגדיר ערך זה; הוא מוגדר על-ידי המערכת.</span><span class="sxs-lookup"><span data-stu-id="5697e-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="5697e-110">לקבלת מידע נוסף, ראה [שדרוג אוטומטי](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="5697e-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="5697e-111">כדי להוריד את הגירסה העדכנית ביותר של חיבור AD תכלת הרקיע, עבור אל [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="5697e-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
