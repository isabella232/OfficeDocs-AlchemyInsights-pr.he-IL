---
title: טכנולוגיית DLP אינו פועל כצפוי
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: eab000e0a850c522ede5f51ae46ba11b87ba4732
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29471995"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="03583-102">טכנולוגיית DLP אינו פועל כצפוי</span><span class="sxs-lookup"><span data-stu-id="03583-102">DLP not working as expected</span></span>

<span data-ttu-id="03583-p101">האם אתה נתקל בבעיות עם **מניעת אובדן נתונים (DLP)** ב- Office 365 אינו פועל כצפוי? אם כן, ודא כי **מדיניות DLP** מותקן כראוי, הנתונים שלך מכיל איזו **מדיניות DLP** מחפש כאשר היא מוערכת.</span><span class="sxs-lookup"><span data-stu-id="03583-p101">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected? If so, make sure that your **DLP policy** is setup correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span> 
  
 <span data-ttu-id="03583-105">**הגדרת DLP:**</span><span class="sxs-lookup"><span data-stu-id="03583-105">**Setting up DLP:**</span></span>
  
<span data-ttu-id="03583-p102">טכנולוגיית DLP מדיניות מאפשרת לך לזהות ולהגן על מידע רגיש בארגון שלך. פריטי מדיניות של טכנולוגיית DLP של תוכנית ההתקנה, השתמש במידע [כאן](https://docs.microsoft.com/en-us/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="03583-p102">DLP policies allows you to identify and protect sensitive information in your organization. To setup DLP policies, use the information [here](https://docs.microsoft.com/en-us/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="03583-108">**מה מדיניות DLP לחפש:**</span><span class="sxs-lookup"><span data-stu-id="03583-108">**What DLP policies look for:**</span></span>
  
<span data-ttu-id="03583-109">בעת שימוש **סוגי מידע רגיש המוכללים** ב- Office 365 האבטחה והתאימות מרכז, מדיניות DLP לחפש תבניות ספציפיות ורכיבי בעת זיהוי סוגי רגישים אלה.</span><span class="sxs-lookup"><span data-stu-id="03583-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span> 
  
- <span data-ttu-id="03583-110">**סוגי מידע רגיש המוכלל:**</span><span class="sxs-lookup"><span data-stu-id="03583-110">**Built-in Sensitive Information Types:**</span></span>
    
    <span data-ttu-id="03583-111">לקבלת מידע אודות סוגי רגיש מוכללים מה מדיניות DLP יחפש בעת זיהוי סוג רגישים, ראה: [חפש אילו סוגי מידע רגיש](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="03583-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>
    
- <span data-ttu-id="03583-112">**סוגי מידע רגיש מותאם אישית:**</span><span class="sxs-lookup"><span data-stu-id="03583-112">**Custom Sensitive Information Types:**</span></span>
    
    <span data-ttu-id="03583-113">אם אתה מנסה ליצור סוגי מידע רגיש מותאם אישית, השתמש במאמר הבא לקבלת מידע אודות אופן היצירה של סוג רגיש מותאם אישית: [צור סוג מותאם אישית מידע רגיש](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="03583-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/en-us/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>
    
 <span data-ttu-id="03583-114">**דוחות**</span><span class="sxs-lookup"><span data-stu-id="03583-114">**Reports:**</span></span>
  
- <span data-ttu-id="03583-115">קבל תובנות נתונים רגישים עם [דוחות מסוג DLP.](https://docs.microsoft.com/en-us/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="03583-115">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/en-us/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>
    
- <span data-ttu-id="03583-116">ראה פרטים ספציפיים של האירוע עם של [דוח תקלה](https://docs.microsoft.com/en-us/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="03583-116">See specific details of the event with an [Incident Report](https://docs.microsoft.com/en-us/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
    

