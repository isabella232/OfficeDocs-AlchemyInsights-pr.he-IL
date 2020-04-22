---
title: DLP לא פועלת כמצופה
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: efb4a19f345fe6b8a1e8bb72abeba4a923c05777
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704414"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="745b5-102">DLP לא פועלת כמצופה</span><span class="sxs-lookup"><span data-stu-id="745b5-102">DLP not working as expected</span></span>

<span data-ttu-id="745b5-103">**חשוב**: בתקופה חסרת תקדים זאת, אנחנו נוקטים בצעדים כדי להבטיח ששירותי SharePoint Online ו- OneDrive יישארו בזמינות גבוהה - לקבלת מידע נוסף, בקר בכתובת[התאמות של תכונה זמנית ב- SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="745b5-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="745b5-104">**הגדרת טכנולוגיית DLP**</span><span class="sxs-lookup"><span data-stu-id="745b5-104">**Setting up DLP**</span></span>

<span data-ttu-id="745b5-105">האם אתה נתקל בבעיות עם **מניעת אובדן נתונים (DLP)** ב-Office 365 לא פועל כצפוי?</span><span class="sxs-lookup"><span data-stu-id="745b5-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="745b5-106">אם כן, ודא **שמדיניות** ה-dlp שלך מוגדרת כראוי ושהנתונים שלך מכילים את המידע **שמדיניות dlp** מחפשת בעת חישובו.</span><span class="sxs-lookup"><span data-stu-id="745b5-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="745b5-107">מדיניות DLP מאפשרת לך לזהות ולהגן על מידע רגיש בארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="745b5-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="745b5-108">כדי להגדיר את מדיניות DLP, השתמש במידע [הנמצא כאן](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="745b5-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="745b5-109">**מה מדיניות DLP מחפשת**</span><span class="sxs-lookup"><span data-stu-id="745b5-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="745b5-110">בעת שימוש **בסוגי המידע הרגישים המובנים** במרכזי האבטחה והתאימות, מדיניות DLP מחפשת תבניות ורכיבים ספציפיים בעת זיהוי סוגים רגישים אלה.</span><span class="sxs-lookup"><span data-stu-id="745b5-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="745b5-111">**סוגי מידע רגישים מוכללים**</span><span class="sxs-lookup"><span data-stu-id="745b5-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="745b5-112">לקבלת מידע אודות הסוגים המובנים המוכללים ומדיניות DLP מחפשת בעת זיהוי הסוג הרגיש, ראה: [מה מחפשים סוגי המידע הרגישים](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="745b5-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="745b5-113">**סוגי מידע רגישים מותאמים אישית**</span><span class="sxs-lookup"><span data-stu-id="745b5-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="745b5-114">אם אתה מנסה ליצור סוגי מידע רגישים מותאמים אישית, השתמש במאמר הבא לקבלת מידע אודות אופן יצירת סוג רגיש מותאם אישית: [יצירת סוג מידע רגיש מותאם אישית](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="745b5-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="745b5-115">**בדיקת מדיניות DLP**</span><span class="sxs-lookup"><span data-stu-id="745b5-115">**Test a DLP policy**</span></span>

<span data-ttu-id="745b5-116">כדי לבדוק את הנתונים שלך באמצעות סוג מידע מובנה או רגיש מותאם אישית, השתמש באפשרות **סוג מבחן** תחת**סוגי מידע רגישים** **לסיווגים** > .</span><span class="sxs-lookup"><span data-stu-id="745b5-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="745b5-117">לקבלת מידע נוסף, ראה [בדיקת סוגי מידע רגישים מותאמים אישית](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="745b5-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="745b5-118">**דוחות**</span><span class="sxs-lookup"><span data-stu-id="745b5-118">**Reports**</span></span>
  
- <span data-ttu-id="745b5-119">קבל תובנות מידע רגישות עם [דוחות DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="745b5-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="745b5-120">ראה פרטים ספציפיים על האירוע עם [דוח אירוע](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="745b5-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
