---
title: טכנולוגיית DLP כלל עבור מספר הביטוח הלאומי אינו פועל
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
ms.openlocfilehash: 757136c39700f12f40f839b29277a59b0e436f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529856"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="fce63-102">בעיות מסוג DLP עם מספרי ביטוח לאומי</span><span class="sxs-lookup"><span data-stu-id="fce63-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="fce63-103">האם אתה נתקל בבעיות עם **מניעת אובדן נתונים (DLP)** אינה פועלת עבור תוכן המכיל של **מספר הביטוח הלאומי (SSN)** בעת שימוש בסוג מידע רגיש ב- Office 365?</span><span class="sxs-lookup"><span data-stu-id="fce63-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="fce63-104">אם כן, ודא כי התוכן שלך מכיל את המידע הדרוש עבור המידע הדרוש מדיניות DLP.</span><span class="sxs-lookup"><span data-stu-id="fce63-104">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="fce63-105">לדוגמה, עבור מדיניות SSN נקבעה עם רמת הביטחון של 85%, הבאות מוערכים ואת אפשרות לזהות עבור הכלל להפעיל:</span><span class="sxs-lookup"><span data-stu-id="fce63-105">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="fce63-106">**[תבנית:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 ספרות, שעשוי להיות בתבנית מעוצב או לא מעוצב</span><span class="sxs-lookup"><span data-stu-id="fce63-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="fce63-107">**[תבנית:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** ארבע פונקציות חפש את SSNs ארבע תבניות שונות:</span><span class="sxs-lookup"><span data-stu-id="fce63-107">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="fce63-108">Func_ssn מוצא SSNs עם טרום-2011 עיצוב חזק המעוצבים באמצעות מקפים או רווחים (או ddd-dd-dddd ddd dddd dd)</span><span class="sxs-lookup"><span data-stu-id="fce63-108">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="fce63-109">Func_unformatted_ssn מוצא SSNs עם טרום-2011 עיצוב חזק שהם לא מעוצב תשע ספרות עוקבים (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="fce63-109">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="fce63-110">Func_randomized_formatted_ssn מוצא SSNs post-2011 המעוצבים באמצעות מקפים או רווחים (או ddd-dd-dddd ddd dddd dd)</span><span class="sxs-lookup"><span data-stu-id="fce63-110">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="fce63-111">Func_randomized_unformatted_ssn מוצא SSNs post-2011 שהם לא מעוצב תשע ספרות עוקבים (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="fce63-111">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="fce63-112">**[בדיקת סיכום:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** לא, קיימת ללא בדיקת סיכום</span><span class="sxs-lookup"><span data-stu-id="fce63-112">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="fce63-113">**[הגדרה:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** מדיניות DLP הוא 85% בטוח כי סוג זה של מידע רגיש זיהה if, בתוך מידת הקירבה של 300 תווים:</span><span class="sxs-lookup"><span data-stu-id="fce63-113">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="fce63-114">[הפונקציה Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) מחפש תוכן התואם את התבנית.</span><span class="sxs-lookup"><span data-stu-id="fce63-114">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="fce63-115">נמצאה מילת מפתח מתוך [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="fce63-115">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="fce63-116">כולל דוגמאות של מילות מפתח: *לאומי, לאומי #, Soc שניה, מספר תעודת זהות* .</span><span class="sxs-lookup"><span data-stu-id="fce63-116">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="fce63-117">לדוגמה, להפעיל דוגמת הבאה עבור המדיניות DLP SSN: **מספר תעודת זהות: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="fce63-117">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="fce63-118">לקבלת מידע נוסף אודות מה נדרש עבור SSNs לאתר עבור התוכן שלך, עיין בסעיף הבא במאמר זה: [מה ה רגיש סוגי מידע מחפשים SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="fce63-118">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="fce63-119">באמצעות סוג אחר מידע רגיש מוכללים, ראה את המאמר הבא לקבלת מידע על מה נדרש עבור סוגים אחרים: [מה ה רגיש סוגי מידע לחפש](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="fce63-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  