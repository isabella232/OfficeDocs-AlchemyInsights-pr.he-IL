---
title: ייתכן שטכנולוגיית DLP זקוקה לסוג מותאם אישית
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 87fcb5c3cc9ccd525265097b66d9d9b3a85c5feb
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977271"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="d3388-102">ייתכן שטכנולוגיית DLP זקוקה לסוג מותאם אישית</span><span class="sxs-lookup"><span data-stu-id="d3388-102">DLP might need a custom type</span></span>

<span data-ttu-id="d3388-103">**חשוב**: במהלך הזמנים חסרי התקדים האלה, אנו נוטלים צעדים כדי להבטיח ששירותי sharepoint online ו-onedrive יישארו זמינים במידה רבה – אנא בקר [בהתאמות התכונות הזמניות של sharepoint online](https://aka.ms/ODSPAdjustments) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="d3388-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="d3388-104">**טכנולוגיית DLP עשויה לדרוש סוג מידע מותאם אישית**</span><span class="sxs-lookup"><span data-stu-id="d3388-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="d3388-105">באמצעות מדיניות של מניעת אובדן נתונים (DLP), באפשרותך לזהות ולהגן על נתונים רגישים בארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="d3388-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="d3388-106">בתרחישים מסוימים, ייתכן שיהיה עליך ליצור סוג מידע **מותאם אישית** משלך כדי להגן על הנתונים של הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="d3388-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="d3388-107">לדוגמה, ייתכן שהארגון שלך יצטרך לזהות ולהגן על מזהי עובדים או על נתונים אחרים בתבנית מסוימת הספציפית לארגון שלך. אם כן, עיין במאמרים הבאים לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="d3388-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="d3388-108">**התאמה אישית של סוג מידע רגיש מוכלל**</span><span class="sxs-lookup"><span data-stu-id="d3388-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="d3388-109">אם סוג מידע רגיש מובנה מתאים לצרכיך עם מספר משודרג בלבד, באפשרותך [להתאים אישית סוג מידע רגיש מוכלל](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="d3388-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="d3388-110">לדוגמה, באפשרותך להוסיף או להסיר מילות מפתח, או להוסיף או להסיר ראיות תומכות כגון תאריך או כתובת.</span><span class="sxs-lookup"><span data-stu-id="d3388-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="d3388-111">**יצירת סוג מידע רגיש מותאם אישית**</span><span class="sxs-lookup"><span data-stu-id="d3388-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="d3388-112">אך אם עליך לזהות ולהגן על סוג אחר של מידע רגיש לחלוטין, באפשרותך [ליצור סוג מידע רגיש ומותאם אישית](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) בממשק המשתמש של מרכז התאימות של אבטחה _ אמפר _.</span><span class="sxs-lookup"><span data-stu-id="d3388-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="d3388-113">**יצירת סוג מידע רגיש מותאם אישית באבטחה _ אמפר _ מרכז התאימות PowerShell**</span><span class="sxs-lookup"><span data-stu-id="d3388-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="d3388-114">לבסוף, אם ממשק המשתמש אינו מספק את כל האפשרויות הדרושות לך, באפשרותך [ליצור סוג מידע רגיש מותאם אישית באבטחה _ אמפר _ מרכז התאימות PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="d3388-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="d3388-115">על-ידי התחלה עם קובץ XML, באפשרותך להשתמש בכל אפשרות זמינה.</span><span class="sxs-lookup"><span data-stu-id="d3388-115">By starting with an XML file, you can use every option available.</span></span>
