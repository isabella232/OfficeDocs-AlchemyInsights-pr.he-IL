---
title: שיתוף עם משתמשים חיצוניים אינו פועל
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36502232"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="851ff-102">פתור בעיות שיתוף תוכן SharePoint עם משתמשים חיצוניים</span><span class="sxs-lookup"><span data-stu-id="851ff-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="851ff-103">ודא כי שיתוף חיצוני מופעלת עבור הארגון שלך:</span><span class="sxs-lookup"><span data-stu-id="851ff-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="851ff-104">עבור אל [שירותי &amp; דף תוספות במרכז admin Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), לחץ על **אתרים**.</span><span class="sxs-lookup"><span data-stu-id="851ff-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="851ff-105">ודא כי ההגדרה מופעלת כדי "On".</span><span class="sxs-lookup"><span data-stu-id="851ff-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="851ff-106">אם נבחר "רק קיימים משתמשים חיצוניים", ודא שמופיע משתמש חיצוני במרכז הניהול של Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="851ff-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="851ff-107">ודא חיצוני שיתופו מופעלת עבור האתר.</span><span class="sxs-lookup"><span data-stu-id="851ff-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="851ff-108">עבור אוסף אתרים קלאסי:</span><span class="sxs-lookup"><span data-stu-id="851ff-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="851ff-109">במרכז הניהול של SharePoint חדש, בחלונית הימנית, לחץ על **אתרים**.</span><span class="sxs-lookup"><span data-stu-id="851ff-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="851ff-110">בחר אתר או אתרים ולאחר ברצועת הכלים, לחץ על **שיתוף**.</span><span class="sxs-lookup"><span data-stu-id="851ff-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="851ff-111">עבור אתר של צוות השייך לקבוצת Office 365, או אתר תקשורת:</span><span class="sxs-lookup"><span data-stu-id="851ff-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="851ff-112">סוגים אלה של האתר החדש יש את אותו שיתוף הגדרת כהגדרה ברחבי הארגון שלך, אלא אם כן הגדרת ארגוני מאפשרת שיתוף קבצים באמצעות קישורים שאינן דורשות הכניסה.</span><span class="sxs-lookup"><span data-stu-id="851ff-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="851ff-113">במקרה זה, האתרים אפשר שיתוף עם משתמשים חיצוניים חדשים וקיימים להיכנס.</span><span class="sxs-lookup"><span data-stu-id="851ff-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="851ff-114">כדי לשנות את ההגדרה עבור אתרים מסוימים, השתמש מרכז הניהול החדש של SharePoint או PowerShell.</span><span class="sxs-lookup"><span data-stu-id="851ff-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="851ff-115">[פרטים נוספים](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="851ff-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="851ff-116">ההגדרה שיתוף חיצוני עבור כל אתר יכול להיות מגבילות יותר את הגדרת הארגון כולו, אך ולקוד לא יותר מההגדרה של הארגון כולו.</span><span class="sxs-lookup"><span data-stu-id="851ff-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

