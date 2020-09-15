---
title: שיתוף עם משתמשים חיצוניים אינו פועל
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691576"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="9ccf8-102">פתרון בעיות בשיתוף תוכן של SharePoint עם משתמשים חיצוניים</span><span class="sxs-lookup"><span data-stu-id="9ccf8-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="9ccf8-103">ודא ששיתוף חיצוני מופעל עבור הארגון שלך:</span><span class="sxs-lookup"><span data-stu-id="9ccf8-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="9ccf8-104">עבור אל [הדף תוספות שירותים &amp; במרכז הניהול של Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)ולחץ על **אתרים**.</span><span class="sxs-lookup"><span data-stu-id="9ccf8-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="9ccf8-105">ודא שההגדרה מופעלת "On".</span><span class="sxs-lookup"><span data-stu-id="9ccf8-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="9ccf8-106">אם האפשרות ' משתמשים חיצוניים קיימים בלבד ' נבחרה, ודא שהמשתמש החיצוני מופיע במרכז הניהול של Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9ccf8-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="9ccf8-107">ודא ששיתוף חיצוני מופעל עבור האתר.</span><span class="sxs-lookup"><span data-stu-id="9ccf8-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="9ccf8-108">עבור אוסף אתרים קלאסי:</span><span class="sxs-lookup"><span data-stu-id="9ccf8-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="9ccf8-109">במרכז הניהול החדש של SharePoint, בחלונית הימנית, לחץ על **אתרים**.</span><span class="sxs-lookup"><span data-stu-id="9ccf8-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="9ccf8-110">בחר את האתר או האתרים, וברצועת הכלים, לחץ על **שיתוף**.</span><span class="sxs-lookup"><span data-stu-id="9ccf8-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="9ccf8-111">עבור אתר צוות השייך לקבוצה של Microsoft 365, או לאתר תקשורת:</span><span class="sxs-lookup"><span data-stu-id="9ccf8-111">For a team site that belongs to a Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="9ccf8-112">סוגי אתרים חדשים אלה כוללים את אותה הגדרת שיתוף כהגדרה של הארגון שלך, אלא אם ההגדרה של הארגון כולה מאפשרת שיתוף קבצים באמצעות קישורים שאינם דורשים כניסה.</span><span class="sxs-lookup"><span data-stu-id="9ccf8-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="9ccf8-113">במקרה זה, האתרים מאפשרים שיתוף עם משתמשים חיצוניים חדשים וקיימים שנכנסים.</span><span class="sxs-lookup"><span data-stu-id="9ccf8-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="9ccf8-114">כדי לשנות את ההגדרה עבור אתרים ספציפיים, השתמש במרכז הניהול החדש של SharePoint או ב-PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9ccf8-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="9ccf8-115">[למידע נוסף](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="9ccf8-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="9ccf8-116">הגדרת השיתוף החיצוני עבור אתר כלשהו יכולה להיות מגבילה יותר מההגדרה הכלל-ארגונית שלך, אך לא יותר מאשר הגדרה של הארגון כולו.</span><span class="sxs-lookup"><span data-stu-id="9ccf8-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

