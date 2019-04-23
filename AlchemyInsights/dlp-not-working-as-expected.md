---
title: טכנולוגיית DLP אינו פועל כצפוי
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 6d8e3e540494e99e42f04080681f46324f2936bd
ms.sourcegitcommit: e87b3f691444db3b9f460c9a3109146dc7ad4f80
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2019
ms.locfileid: "31869560"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="c2a5c-102">טכנולוגיית DLP אינו פועל כצפוי</span><span class="sxs-lookup"><span data-stu-id="c2a5c-102">DLP not working as expected</span></span>


<span data-ttu-id="c2a5c-103">האם אתה נתקל בבעיות עם **מניעת אובדן נתונים (DLP)** ב- Office 365 אינו פועל כצפוי?</span><span class="sxs-lookup"><span data-stu-id="c2a5c-103">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="c2a5c-104">אם כן, ודא כי **מדיניות DLP** שלך מוגדר כראוי, הנתונים שלך מכיל איזו **מדיניות DLP** מחפש כאשר היא מוערכת.</span><span class="sxs-lookup"><span data-stu-id="c2a5c-104">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span> 
  
 <span data-ttu-id="c2a5c-105">**הגדרת DLP:**</span><span class="sxs-lookup"><span data-stu-id="c2a5c-105">**Setting up DLP:**</span></span>
  
<span data-ttu-id="c2a5c-106">טכנולוגיית DLP מדיניות מאפשרת לך לזהות ולהגן על מידע רגיש בארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="c2a5c-106">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="c2a5c-107">פריטי מדיניות של טכנולוגיית DLP של תוכנית ההתקנה, השתמש במידע [כאן](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="c2a5c-107">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="c2a5c-108">**מה מדיניות DLP לחפש:**</span><span class="sxs-lookup"><span data-stu-id="c2a5c-108">**What DLP policies look for:**</span></span>
  
<span data-ttu-id="c2a5c-109">בעת שימוש **סוגי מידע רגיש המוכללים** ב- Office 365 האבטחה והתאימות מרכז, מדיניות DLP לחפש תבניות ספציפיות ורכיבי בעת זיהוי סוגי רגישים אלה.</span><span class="sxs-lookup"><span data-stu-id="c2a5c-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span> 
  
- <span data-ttu-id="c2a5c-110">**סוגי מידע רגיש המוכלל:**</span><span class="sxs-lookup"><span data-stu-id="c2a5c-110">**Built-in Sensitive Information Types:**</span></span>
    
    <span data-ttu-id="c2a5c-111">לקבלת מידע אודות סוגי רגיש מוכללים מה מדיניות DLP יחפש בעת זיהוי סוג רגישים, ראה: [חפש אילו סוגי מידע רגיש](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="c2a5c-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>
    
- <span data-ttu-id="c2a5c-112">**סוגי מידע רגיש מותאם אישית:**</span><span class="sxs-lookup"><span data-stu-id="c2a5c-112">**Custom Sensitive Information Types:**</span></span>
    
    <span data-ttu-id="c2a5c-113">אם אתה מנסה ליצור סוגי מידע רגיש מותאם אישית, השתמש במאמר הבא לקבלת מידע אודות אופן היצירה של סוג רגיש מותאם אישית: [צור סוג מותאם אישית מידע רגיש](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="c2a5c-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>
    
 <span data-ttu-id="c2a5c-114">**דוחות:**</span><span class="sxs-lookup"><span data-stu-id="c2a5c-114">**Reports:**</span></span>
  
- <span data-ttu-id="c2a5c-115">קבל תובנות נתונים רגישים עם [דוחות מסוג DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="c2a5c-115">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>
    
- <span data-ttu-id="c2a5c-116">ראה פרטים ספציפיים של האירוע עם של [דוח תקלה](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="c2a5c-116">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
    

