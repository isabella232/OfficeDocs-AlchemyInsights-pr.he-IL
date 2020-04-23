---
title: 932 שדרוג השדרוג
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766494"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="1421f-102">לשדרג התכלת להתחבר</span><span class="sxs-lookup"><span data-stu-id="1421f-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="1421f-103">כברירת מחדל, השדרוג האוטומטי מאופשר לחיבור תכלת לספירה, המסייע להבטיח שאתה מפעיל את הגירסה העדכנית ביותר.</span><span class="sxs-lookup"><span data-stu-id="1421f-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="1421f-104">כדי לאמת את הגדרות השדרוג האוטומטי, השתמש ב **-Cmdlet קבל-Adsynpכתה** ב תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="1421f-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="1421f-105">ה-cmdlet יחזיר אחד מהערכים הבאים:</span><span class="sxs-lookup"><span data-stu-id="1421f-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="1421f-106">**זמין**: שדרוג אוטומטי מאופשר.</span><span class="sxs-lookup"><span data-stu-id="1421f-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="1421f-107">לא **זמין**: שדרוג אוטומטי אינו זמין.</span><span class="sxs-lookup"><span data-stu-id="1421f-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="1421f-108">**מושעה**: המערכת אינה זכאית עוד לקבל שדרוגים אוטומטיים.</span><span class="sxs-lookup"><span data-stu-id="1421f-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="1421f-109">אין באפשרותך לקבוע את התצורה של ערך זה; היא מוגדרת על-ידי המערכת.</span><span class="sxs-lookup"><span data-stu-id="1421f-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="1421f-110">לקבלת מידע נוסף, ראה [שדרוג אוטומטי](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="1421f-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="1421f-111">כדי להוריד את הגרסה העדכנית ביותר של תכלת [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)AD התחבר, עבור אל.</span><span class="sxs-lookup"><span data-stu-id="1421f-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
