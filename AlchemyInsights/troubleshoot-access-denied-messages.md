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
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704895"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="cecee-102">פתרון בעיות בהודעות של Access שנדחו</span><span class="sxs-lookup"><span data-stu-id="cecee-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="cecee-103">אם מישהו קיבל הודעת "הגישה נדחתה" לתיקיה משותפת ב-SharePoint, ייתכן שמנהל אוסף האתרים הזמין את ' מצב נעילה של הרשאות משתמש מוגבל לגישה מוגבלת '.</span><span class="sxs-lookup"><span data-stu-id="cecee-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="cecee-104">כדי לבטל זאת:</span><span class="sxs-lookup"><span data-stu-id="cecee-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="cecee-105">אתר את האתר, לחץ על סמל הגדרות ולאחר מכן לחץ על **הגדרות האתר**.</span><span class="sxs-lookup"><span data-stu-id="cecee-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="cecee-106">תחת **ניהול אוסף אתרים**, לחץ על **תכונות אוסף אתרים**.</span><span class="sxs-lookup"><span data-stu-id="cecee-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="cecee-107">לצד **מצב נעילה של הרשאות משתמש בגישה מוגבלת**, לחץ על **בטל הפעלה**.</span><span class="sxs-lookup"><span data-stu-id="cecee-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="cecee-108">הודעת גישה שנדחתה יכולה להתרחש גם עבור תיקיות משותפות אם האתר הוא אתר פרסום.</span><span class="sxs-lookup"><span data-stu-id="cecee-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="cecee-109">לקבלת מידע, ראה [Access נדחה בעת גישה לתיקיה משותפת](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span><span class="sxs-lookup"><span data-stu-id="cecee-109">For info, see [Access Denied when accessing a shared folder](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span></span>
  
<span data-ttu-id="cecee-110">אם מישהו קיבל הודעת "הגישה נדחתה" בעת ניסיון להציג בקשות גישה, המשתמש צריך להתווסף כמנהל אוסף אתרים או כחבר בקבוצה ' בעלים ' עבור האתר.</span><span class="sxs-lookup"><span data-stu-id="cecee-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="cecee-111">לקבלת מידע נוסף, ראה [הרשימה בקשות לגישה נדחתה](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="cecee-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="cecee-112">אם משתמש קיבל הודעת "הגישה נדחתה" לאחר הסרת ההודעה מ-Active Directory מקומי ולאחר מכן נוסף, ראה [Access נדחה בעת סינכרון חשבון משתמש ל-Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="cecee-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

