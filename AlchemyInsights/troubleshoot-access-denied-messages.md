---
title: פתרון בעיות בהודעות שנדחו על-ידי Access
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 05d12aee49b449e8a29e84021b41298fb9983859
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050706"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="d3123-102">פתרון בעיות בהודעות שנדחו על-ידי Access</span><span class="sxs-lookup"><span data-stu-id="d3123-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="d3123-103">אם מישהו קיבל הודעה של ' הגישה נדחתה ' לתיקיה משותפת ב-SharePoint, ייתכן שמנהל אוסף האתרים הפך את האפשרות "מצב נעילה של הרשאת משתמש בגישה מוגבלת".</span><span class="sxs-lookup"><span data-stu-id="d3123-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="d3123-104">כדי לבטל את הפעולה:</span><span class="sxs-lookup"><span data-stu-id="d3123-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="d3123-105">דפדף אל האתר, לחץ על הסמל הגדרות ולאחר מכן לחץ על **הגדרות אתר**.</span><span class="sxs-lookup"><span data-stu-id="d3123-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="d3123-106">תחת **ניהול אוסף אתרים**, לחץ על **תכונות של אוסף אתרים**.</span><span class="sxs-lookup"><span data-stu-id="d3123-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="d3123-107">לצד **מצב נעילה של הרשאת משתמש מוגבל של גישה מוגבלת**, לחץ על **בטל הפעלתו**.</span><span class="sxs-lookup"><span data-stu-id="d3123-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="d3123-108">הודעה של גישה שנדחתה יכולה להתרחש גם עבור תיקיות משותפות אם האתר הוא אתר פרסום.</span><span class="sxs-lookup"><span data-stu-id="d3123-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="d3123-109">לקבלת מידע, ראה [גישה נדחתה בעת גישה לתיקיה משותפת](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="d3123-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="d3123-110">אם מישהו קיבל הודעה של ' הגישה נדחתה ' בעת ניסיון להציג בקשות גישה, יש להוסיף את המשתמש כמנהל אוסף אתרים או כחבר בקבוצה ' בעלים ' עבור האתר.</span><span class="sxs-lookup"><span data-stu-id="d3123-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="d3123-111">לקבלת מידע נוסף, ראה [גישה אל רשימת בקשות access שנדחתה](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="d3123-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="d3123-112">אם משתמש קיבל הודעה מתוך ' הגישה נדחתה ' לאחר שהוסרו מ-Active Directory ולאחר מכן התווספה חזרה, ראה [גישה נדחתה כאשר חשבון משתמש מסונכרנת ל-Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="d3123-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

