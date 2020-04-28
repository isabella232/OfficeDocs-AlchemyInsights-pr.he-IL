---
title: שיתוף עם משתמשים חיצוניים אינו פועל
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 37da77c73b3abbdcf9cb2b9c4c43f31eea3c0a49
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/27/2020
ms.locfileid: "43913003"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="91f64-102">תיקון בעיות בשיתוף תוכן SharePoint עם משתמשים חיצוניים</span><span class="sxs-lookup"><span data-stu-id="91f64-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="91f64-103">ודא ששיתוף חיצוני מופעל עבור הארגון שלך:</span><span class="sxs-lookup"><span data-stu-id="91f64-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="91f64-104">עבור אל [דף התוספות של &amp; שירותים במרכז הניהול של Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), ולחץ על **אתרים**.</span><span class="sxs-lookup"><span data-stu-id="91f64-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="91f64-105">ודא שההגדרה הפכה ל-"On".</span><span class="sxs-lookup"><span data-stu-id="91f64-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="91f64-106">אם נבחר "רק משתמשים חיצוניים קיימים", ודא שהמשתמש החיצוני מופיע במרכז הניהול של Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="91f64-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="91f64-107">ודא ששיתוף חיצוני מופעל עבור האתר.</span><span class="sxs-lookup"><span data-stu-id="91f64-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="91f64-108">לקבלת אוסף אתרים קלאסי:</span><span class="sxs-lookup"><span data-stu-id="91f64-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="91f64-109">במרכז הניהול החדש של SharePoint, בחלונית הימנית, לחץ על **אתרים**.</span><span class="sxs-lookup"><span data-stu-id="91f64-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="91f64-110">בחר את האתר או האתרים, וברצועת הכלים, לחץ על **שיתוף**.</span><span class="sxs-lookup"><span data-stu-id="91f64-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="91f64-111">עבור אתר צוות השייך לקבוצת Microsoft 365 או לאתר תקשורת:</span><span class="sxs-lookup"><span data-stu-id="91f64-111">For a team site that belongs to an Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="91f64-112">לסוגי אתרים חדשים אלה יש הגדרת שיתוף זהה לזו של הגדרת הארגון שלך, אלא אם כן ההגדרה כלל-ארגונית מאפשרת שיתוף קבצים באמצעות קישורים שאינם דורשים כניסה.</span><span class="sxs-lookup"><span data-stu-id="91f64-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="91f64-113">במקרה זה, האתרים מאפשרים שיתוף עם משתמשים חיצוניים חדשים וקיימים החותמים.</span><span class="sxs-lookup"><span data-stu-id="91f64-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="91f64-114">כדי לשנות את ההגדרה עבור אתרים מסוימים, השתמש במרכז הניהול החדש של SharePoint או ב-PowerShell.</span><span class="sxs-lookup"><span data-stu-id="91f64-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="91f64-115">[למידע נוסף](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="91f64-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="91f64-116">הגדרת השיתוף החיצוני עבור כל אתר יכולה להיות מגבילה יותר מההגדרה הכלל-ארגונית, אך לא יותר מתירני מאשר ההגדרה הכלל-ארגונית.</span><span class="sxs-lookup"><span data-stu-id="91f64-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

