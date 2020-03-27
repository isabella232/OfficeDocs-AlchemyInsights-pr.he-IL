---
title: כלל DLP עבור SSN אינו פועל
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 4ec0df9d4954a8c65f0c34188d285dd8cf44a4f2
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977307"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="4b990-102">DLP בעיות עם מספרי ביטוח לאומי</span><span class="sxs-lookup"><span data-stu-id="4b990-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="4b990-103">**חשוב**: במהלך הזמנים חסרי התקדים האלה, אנו נוטלים צעדים כדי להבטיח ששירותי sharepoint online ו-onedrive יישארו זמינים במידה רבה – אנא בקר [בהתאמות התכונות הזמניות של sharepoint online](https://aka.ms/ODSPAdjustments) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="4b990-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="4b990-104">**DLP בעיות עם SSNs**</span><span class="sxs-lookup"><span data-stu-id="4b990-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="4b990-105">האם אתה נתקל בבעיות עם **מניעת אובדן נתונים (DLP)** שאינם פועלים עבור תוכן המכיל **מספר תעודת זהות (SSN)** בעת שימוש בסוג מידע רגיש ב-Office 365?</span><span class="sxs-lookup"><span data-stu-id="4b990-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="4b990-106">אם כן, ודא שהתוכן שלך מכיל את המידע הדרוש עבור מה שמדיניות ה-DLP מחפשת.</span><span class="sxs-lookup"><span data-stu-id="4b990-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="4b990-107">לדוגמה, עבור מדיניות SSN המוגדרת עם רמת ביטחון של 85%, ההערכה הבאה מוערכת ויש לאתרם כדי שהכלל יפעיל:</span><span class="sxs-lookup"><span data-stu-id="4b990-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="4b990-108">**[תבנית:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 ספרות, שעשויות להיות בתבנית מעוצבת או לא מאותחלת</span><span class="sxs-lookup"><span data-stu-id="4b990-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="4b990-109">**[תבנית:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** ארבע פונקציות מחפש SSNs בארבעה דפוסים שונים:</span><span class="sxs-lookup"><span data-stu-id="4b990-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="4b990-110">Func_ssn מוצא SSNs עם עיצוב חזק של pre-2011 המעוצבים באמצעות מקפים או רווחים (ddd-dd-dddd או ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="4b990-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="4b990-111">Func_unformatted_ssn מוצא SSNs עם עיצוב חזק של pre-2011 שאינם מתוכנתים כתשע ספרות רצופות (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="4b990-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="4b990-112">Func_randomized_formatted_ssn מאתרת SSNs שלאחר 2011 המעוצבים באמצעות מקפים או רווחים (ddd-dd-dddd או ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="4b990-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="4b990-113">Func_randomized_unformatted_ssn מוצאת SSNs שלאחר 2011 שאינם מאותחלת כתשע ספרות רצופות (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="4b990-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="4b990-114">**[בדיקת סיכום:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** לא, אין בדיקת סיכום</span><span class="sxs-lookup"><span data-stu-id="4b990-114">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="4b990-115">**[הגדרה:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** מדיניות DLP היא 85% בטוחה שהיא זיהתה סוג זה של מידע רגיש אם, בסמיכות של 300 תווים:</span><span class="sxs-lookup"><span data-stu-id="4b990-115">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="4b990-116">[הפונקציה Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) מאתרת תוכן התואם לתבנית.</span><span class="sxs-lookup"><span data-stu-id="4b990-116">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="4b990-117">נמצאה מילת מפתח מ- [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="4b990-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="4b990-118">דוגמאות של מילות מפתח כולל: *ביטוח לאומי, ביטוח לאומי, Soc שניה, SSN* .</span><span class="sxs-lookup"><span data-stu-id="4b990-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="4b990-119">לדוגמה, הדוגמה הבאה תפעיל את מדיניות DLP SSN: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="4b990-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="4b990-120">לקבלת מידע נוסף אודות הדרוש עבור SSNs שיזוהו עבור התוכן שלך, עיין בסעיף הבא במאמר זה: [מה סוגי המידע הרגישים מחפשים SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="4b990-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="4b990-121">באמצעות סוג מידע רגיש ומובנה שונה, עיין במאמר הבא לקבלת מידע אודות הדרוש עבור סוגים אחרים: [מה סוגי המידע הרגישים מחפשים](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="4b990-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  