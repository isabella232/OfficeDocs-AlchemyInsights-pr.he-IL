---
title: כלל DLP של מספר חשבון בנק בארה ב אינו פועל
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: bb7d8ca91af73fa4ebed5992ec848128beb18830
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977163"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="abe47-102">DLP בעיות עם מספרי חשבונות בנק בארה ב</span><span class="sxs-lookup"><span data-stu-id="abe47-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="abe47-103">**חשוב**: במהלך הזמנים חסרי התקדים האלה, אנו נוטלים צעדים כדי להבטיח ששירותי sharepoint online ו-onedrive יישארו זמינים במידה רבה – אנא בקר [בהתאמות התכונות הזמניות של sharepoint online](https://aka.ms/ODSPAdjustments) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="abe47-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="abe47-104">**DLP בעיות עם מספרי חשבונות בנק בארה ב**</span><span class="sxs-lookup"><span data-stu-id="abe47-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="abe47-105">האם אתה נתקל בבעיות עם **מניעת אובדן נתונים (DLP)** שאינם פועלים עבור תוכן המכיל **מספר חשבון בנק בארה** ב בעת שימוש בסוג מידע רגיש של DLP ב-O365?</span><span class="sxs-lookup"><span data-stu-id="abe47-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="abe47-106">אם כן, ודא שהתוכן שלך מכיל את המידע הדרוש עבור מה שמדיניות DLP מחפשת בעת חישובו.</span><span class="sxs-lookup"><span data-stu-id="abe47-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="abe47-107">לדוגמה, עבור מדיניות **מספר חשבון בנק של ארה"ב** המוגדרת ברמת ביטחון של 85%, ההערכה הבאה מוערכת ויש לאתרם כדי שהכלל יפעיל:</span><span class="sxs-lookup"><span data-stu-id="abe47-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="abe47-108">**[תבנית:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 ספרות</span><span class="sxs-lookup"><span data-stu-id="abe47-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="abe47-109">**[תבנית:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 ספרות רצופות.</span><span class="sxs-lookup"><span data-stu-id="abe47-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="abe47-110">**[בדיקת סיכום:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** לא, אין בדיקת סיכום</span><span class="sxs-lookup"><span data-stu-id="abe47-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="abe47-111">**[הגדרה:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** מדיניות DLP היא 75% בטוחה שהיא זיהתה סוג זה של מידע רגיש אם, בסמיכות של 300 תווים:</span><span class="sxs-lookup"><span data-stu-id="abe47-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="abe47-112">הביטוי הרגיל Regex_usa_bank_account_number מוצא תוכן התואם לתבנית</span><span class="sxs-lookup"><span data-stu-id="abe47-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="abe47-113">נמצאה מילת מפתח מ-Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="abe47-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="abe47-114">לדוגמה, הדוגמה הבאה תפעיל את מדיניות **מספר חשבון הבנק של ארה"ב** : בדיקת חשבון 78344011</span><span class="sxs-lookup"><span data-stu-id="abe47-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="abe47-115">לקבלת מידע נוסף אודות הדרוש עבור **מספר חשבון בנק של ארה"ב** שיזוהה עבור התוכן שלך, עיין בסעיף הבא במאמר זה: [מה סוגי המידע הרגישים מחפשים מספר חשבון בנק US](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="abe47-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="abe47-116">באמצעות סוג מידע רגיש ומובנה שונה, עיין במאמר הבא לקבלת מידע אודות הדרוש עבור סוגים אחרים: [מה סוגי המידע הרגישים מחפשים](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="abe47-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  