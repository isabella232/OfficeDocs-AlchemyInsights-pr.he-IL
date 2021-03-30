---
title: בעיות של בעלים של רישום אפליקציה
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404774"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="0c32c-102">בעיות של בעלים של רישום אפליקציה</span><span class="sxs-lookup"><span data-stu-id="0c32c-102">App Registration Owner issues</span></span>

<span data-ttu-id="0c32c-103">להלן השיטות הזמינות להוספת מנהלים כבעלים עבור רישומי אפליקציות:</span><span class="sxs-lookup"><span data-stu-id="0c32c-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="0c32c-104">שימוש במודול Azure AD PowerShell -</span><span class="sxs-lookup"><span data-stu-id="0c32c-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="0c32c-105">הפניה: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="0c32c-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="0c32c-106">שימוש ב- Azure CLI - `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="0c32c-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="0c32c-107">הפניה: [הבעלים של אפליקציית המודעות az](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="0c32c-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="0c32c-108">שימוש ב- MS Graph -</span><span class="sxs-lookup"><span data-stu-id="0c32c-108">Using MS Graph -</span></span>

    <span data-ttu-id="0c32c-109">הפניה: [הוספת בעלים - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="0c32c-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="0c32c-110">שימוש בפורטל Azure AD - נווט [אל portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > בחר את היישום שלך > בעלים > הוסף בעלים</span><span class="sxs-lookup"><span data-stu-id="0c32c-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="0c32c-111">**לא ניתן להציג את היישום שלך בלהב 'רישומי אפליקציה' למרות שאתה הבעלים של יישום זה?**</span><span class="sxs-lookup"><span data-stu-id="0c32c-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="0c32c-112">הבעלים של יישום אינו תפקיד ניהולי.</span><span class="sxs-lookup"><span data-stu-id="0c32c-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="0c32c-113">אם ההגדרה [הגבל גישה לפורטל](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) הניהול של Azure AD זמינה, רק מנהל המערכת יוכל להציג את היישומים בפורטל רישום יישומים.</span><span class="sxs-lookup"><span data-stu-id="0c32c-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="0c32c-114">כדי שהבעלים יוכל להציג את היישומים, הפוך הגדרה זו ללא זמינה (הגדר הגדרה זו ללא) או הקצה תפקיד מנהל מערכת לבעלים עבור היישום הספציפי בלבד.</span><span class="sxs-lookup"><span data-stu-id="0c32c-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="0c32c-115">עם זאת, תדרוש רשיון Azure AD Premium P2 ותאפשר [ניהול זהויות מורשה.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)</span><span class="sxs-lookup"><span data-stu-id="0c32c-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
