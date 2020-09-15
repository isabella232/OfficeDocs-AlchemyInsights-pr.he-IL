---
title: פתרון בעיות בהודעות של Access שנדחו
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3550081a12379f73725253214a2c2d44974ab740
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690784"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="dd2ab-102">פתרון בעיות בהודעות של Access שנדחו</span><span class="sxs-lookup"><span data-stu-id="dd2ab-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="dd2ab-103">אם מישהו קיבל הודעת "הגישה נדחתה" לתיקיה משותפת ב-SharePoint, ייתכן שמנהל אוסף האתרים הזמין את ' מצב נעילה של הרשאות משתמש מוגבל לגישה מוגבלת '.</span><span class="sxs-lookup"><span data-stu-id="dd2ab-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="dd2ab-104">כדי לבטל זאת:</span><span class="sxs-lookup"><span data-stu-id="dd2ab-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="dd2ab-105">אתר את האתר, לחץ על סמל הגדרות ולאחר מכן לחץ על **הגדרות האתר**.</span><span class="sxs-lookup"><span data-stu-id="dd2ab-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="dd2ab-106">תחת **ניהול אוסף אתרים**, לחץ על **תכונות אוסף אתרים**.</span><span class="sxs-lookup"><span data-stu-id="dd2ab-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="dd2ab-107">לצד **מצב נעילה של הרשאות משתמש בגישה מוגבלת**, לחץ על **בטל הפעלה**.</span><span class="sxs-lookup"><span data-stu-id="dd2ab-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="dd2ab-108">הודעת גישה שנדחתה יכולה להתרחש גם עבור תיקיות משותפות אם האתר הוא אתר פרסום.</span><span class="sxs-lookup"><span data-stu-id="dd2ab-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="dd2ab-109">לקבלת מידע, ראה [Access נדחה בעת גישה לתיקיה משותפת](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="dd2ab-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="dd2ab-110">אם מישהו קיבל הודעת "הגישה נדחתה" בעת ניסיון להציג בקשות גישה, המשתמש צריך להתווסף כמנהל אוסף אתרים או כחבר בקבוצה ' בעלים ' עבור האתר.</span><span class="sxs-lookup"><span data-stu-id="dd2ab-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="dd2ab-111">לקבלת מידע נוסף, ראה [הרשימה בקשות לגישה נדחתה](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="dd2ab-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="dd2ab-112">אם משתמש קיבל הודעת "הגישה נדחתה" לאחר הסרת ההודעה מ-Active Directory מקומי ולאחר מכן נוסף, ראה [Access נדחה בעת סינכרון חשבון משתמש ל-Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="dd2ab-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

