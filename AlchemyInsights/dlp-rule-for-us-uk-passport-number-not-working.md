---
title: כלל DLP של מספר דרכון בארה ב/בבריטניה אינו פועל
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 3d3b7dc2d9510376bc9eef6ec69b87ad7c681b05
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507299"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="0f467-102">בעיות עם מספרי הדרכון של DLP-US/בריטניה</span><span class="sxs-lookup"><span data-stu-id="0f467-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="0f467-103">**חשוב**: בתקופה חסרת תקדים זאת, אנחנו נוקטים בצעדים כדי להבטיח ששירותי SharePoint Online ו- OneDrive יישארו בזמינות גבוהה - לקבלת מידע נוסף, בקר בכתובת[התאמות של תכונה זמנית ב- SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="0f467-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="0f467-104">**בעיות DLP של מספרי דרכון בארה ב/בבריטניה**</span><span class="sxs-lookup"><span data-stu-id="0f467-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="0f467-105">האם אתה נתקל בבעיות עם **מניעת אובדן נתונים (DLP)** שאינה פועלת עבור תוכן המכיל **מספר דרכון בארה ב/בבריטניה** בעת שימוש בסוג מידע רגיש של DLP ב-O365?</span><span class="sxs-lookup"><span data-stu-id="0f467-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="0f467-106">אם כן, ודא שהתוכן שלך מכיל את המידע הדרוש עבור מה שמדיניות DLP מחפשת בעת חישובו.</span><span class="sxs-lookup"><span data-stu-id="0f467-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="0f467-107">לדוגמה, עבור מדיניות **מספר דרכון של ארה"ב/UK** המוגדרת עם רמת ביטחון של 75%, ההערכה הבאה מוערכת ויש לאתרם כדי שהכלל יפעיל</span><span class="sxs-lookup"><span data-stu-id="0f467-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="0f467-108">[**תבנית:**](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77) תשע ספרות</span><span class="sxs-lookup"><span data-stu-id="0f467-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="0f467-109">[**תבנית:**](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77) תשע ספרות רצופות</span><span class="sxs-lookup"><span data-stu-id="0f467-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="0f467-110">[**בדיקת סיכום:**](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76) לא, אין בדיקת סיכום</span><span class="sxs-lookup"><span data-stu-id="0f467-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="0f467-111">[**הגדרה:**](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77) מדיניות DLP היא 75% בטוחה שהיא זיהתה סוג זה של מידע רגיש אם, בסמיכות של 300 תווים:</span><span class="sxs-lookup"><span data-stu-id="0f467-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="0f467-112">הפונקציה Func_usa_uk_passport מאתרת תוכן התואם לתבנית.</span><span class="sxs-lookup"><span data-stu-id="0f467-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="0f467-113">נמצאה מילת מפתח מKeyword_passport.</span><span class="sxs-lookup"><span data-stu-id="0f467-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="0f467-114">לדוגמה, הדוגמה הבאה תפעיל את מדיניות **מספר הדרכון ארה ב/בריטניה** : דרכון מספר 123456789 בארה ב</span><span class="sxs-lookup"><span data-stu-id="0f467-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="0f467-115">לקבלת מידע נוסף אודות הנדרש עבור מספר Passport של ארה ב/בריטניה שיזוהה עבור התוכן שלך, עיין בסעיף הבא במאמר זה: [מה סוגי המידע הרגישים מחפשים מספר דרכון בארה ב/בריטניה](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="0f467-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="0f467-116">באמצעות סוג מידע רגיש ומובנה שונה, עיין במאמר הבא לקבלת מידע אודות הדרוש עבור סוגים אחרים: [מה סוגי המידע הרגישים מחפשים](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="0f467-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  