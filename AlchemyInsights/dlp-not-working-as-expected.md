---
title: DLP אינו פועל כמצופה
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707811"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="f9ec9-102">DLP אינו פועל כמצופה</span><span class="sxs-lookup"><span data-stu-id="f9ec9-102">DLP not working as expected</span></span>

<span data-ttu-id="f9ec9-103">**חשוב**: בתקופה חסרת תקדים זאת, אנחנו נוקטים בצעדים כדי להבטיח ששירותי SharePoint Online ו- OneDrive יישארו בזמינות גבוהה - לקבלת מידע נוסף, בקר בכתובת [התאמות של תכונה זמנית ב- SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="f9ec9-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="f9ec9-104">**הגדרת DLP**</span><span class="sxs-lookup"><span data-stu-id="f9ec9-104">**Setting up DLP**</span></span>

<span data-ttu-id="f9ec9-105">האם אתה נתקל בבעיות **במניעת אובדן נתונים (DLP)** ב-Office 365 שאינו פועל כצפוי?</span><span class="sxs-lookup"><span data-stu-id="f9ec9-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="f9ec9-106">אם כן, ודא **שמדיניות** ה-dlp שלך מוגדרת כהלכה, ושהנתונים שלך מכילים את מראה **המדיניות של dlp** כאשר היא מוערכת.</span><span class="sxs-lookup"><span data-stu-id="f9ec9-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="f9ec9-107">מדיניות DLP מאפשרת לך לזהות ולהגן על מידע רגיש בארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="f9ec9-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="f9ec9-108">כדי להגדיר את מדיניות DLP, השתמש [במידע](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)שלהלן.</span><span class="sxs-lookup"><span data-stu-id="f9ec9-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).</span></span>
  
 <span data-ttu-id="f9ec9-109">**מה מדיניות DLP מחפשת**</span><span class="sxs-lookup"><span data-stu-id="f9ec9-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="f9ec9-110">בעת שימוש **בסוגי המידע המובנים המובנים** במרכזי האבטחה והתאימות, מדיניות DLP מחפשת אחר תבניות ורכיבים ספציפיים בעת זיהוי סוגי נתונים רגישים אלה.</span><span class="sxs-lookup"><span data-stu-id="f9ec9-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="f9ec9-111">**סוגי מידע רגישים מוכללים**</span><span class="sxs-lookup"><span data-stu-id="f9ec9-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="f9ec9-112">לקבלת מידע אודות הסוגים המוכללים הרגישים ומהו המראה של מדיניות DLP בעת זיהוי הסוג הרגיש, ראה: [מה סוגי המידע הרגישים מחפשים](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="f9ec9-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="f9ec9-113">**סוגי מידע רגישים מותאמים אישית**</span><span class="sxs-lookup"><span data-stu-id="f9ec9-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="f9ec9-114">אם אתה מנסה ליצור סוגי מידע רגישים מותאמים אישית, השתמש במאמר הבא לקבלת מידע אודות אופן היצירה של סוג רגיש מותאם אישית: [יצירת סוג מידע רגיש מותאם אישית](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="f9ec9-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="f9ec9-115">**בדיקת מדיניות DLP**</span><span class="sxs-lookup"><span data-stu-id="f9ec9-115">**Test a DLP policy**</span></span>

<span data-ttu-id="f9ec9-116">כדי לבדוק את הנתונים שלך באמצעות סוג מידע רגיש מוכלל או מותאם אישית, השתמש באפשרות **סוג בדיקה** תחת **סיווג**  >  **סוגי מידע רגישים**.</span><span class="sxs-lookup"><span data-stu-id="f9ec9-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="f9ec9-117">לקבלת מידע נוסף, ראה [בדיקת סוגי מידע רגישים מותאמים אישית](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="f9ec9-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="f9ec9-118">**דוחות**</span><span class="sxs-lookup"><span data-stu-id="f9ec9-118">**Reports**</span></span>
  
- <span data-ttu-id="f9ec9-119">קבל תובנות רגישות של נתונים באמצעות [דוחות DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="f9ec9-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="f9ec9-120">ראה פרטים ספציפיים של האירוע באמצעות [דוח מאורע](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="f9ec9-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
