---
title: טכנולוגיית DLP כלל עבור מספר הביטוח הלאומי אינו פועל
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b92d122b774d97cd2e44cc0880dc5001065b57cc
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29472886"
---
<span data-ttu-id="026c0-p101">האם אתה נתקל בבעיות עם **מניעת אובדן נתונים (DLP)** אינה פועלת עבור תוכן המכיל של **מספר הביטוח הלאומי (SSN)** בעת שימוש בסוג מידע רגיש ב- Office 365? אם כן, ודא כי התוכן שלך מכיל את המידע הדרוש עבור המידע הדרוש מדיניות DLP.</span><span class="sxs-lookup"><span data-stu-id="026c0-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365? If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="026c0-104">לדוגמה, עבור מדיניות SSN נקבעה עם רמת הביטחון של 85%, הבאות מוערכים ואת אפשרות לזהות עבור הכלל להפעיל:</span><span class="sxs-lookup"><span data-stu-id="026c0-104">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="026c0-105">**[תבנית:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 ספרות, שעשוי להיות בתבנית מעוצב או לא מעוצב</span><span class="sxs-lookup"><span data-stu-id="026c0-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span> 
    
- <span data-ttu-id="026c0-106">**[תבנית:](https://msconnect.microsoft.com/https:/docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** ארבע פונקציות חפש את SSNs ארבע תבניות שונות:</span><span class="sxs-lookup"><span data-stu-id="026c0-106">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span> 
    
  - <span data-ttu-id="026c0-107">Func_ssn מוצא SSNs עם טרום-2011 עיצוב חזק המעוצבים באמצעות מקפים או רווחים (או ddd-dd-dddd ddd dddd dd)</span><span class="sxs-lookup"><span data-stu-id="026c0-107">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="026c0-108">Func_unformatted_ssn מוצא SSNs עם טרום-2011 עיצוב חזק שהם לא מעוצב תשע ספרות עוקבים (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="026c0-108">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
  - <span data-ttu-id="026c0-109">Func_randomized_formatted_ssn מוצא SSNs post-2011 המעוצבים באמצעות מקפים או רווחים (או ddd-dd-dddd ddd dddd dd)</span><span class="sxs-lookup"><span data-stu-id="026c0-109">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="026c0-110">Func_randomized_unformatted_ssn מוצא SSNs post-2011 שהם לא מעוצב תשע ספרות עוקבים (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="026c0-110">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
- <span data-ttu-id="026c0-111">**[בדיקת סיכום:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** לא, קיימת ללא בדיקת סיכום</span><span class="sxs-lookup"><span data-stu-id="026c0-111">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="026c0-112">**[הגדרה:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** מדיניות DLP הוא 85% בטוח כי סוג זה של מידע רגיש זיהה if, בתוך מידת הקירבה של 300 תווים:</span><span class="sxs-lookup"><span data-stu-id="026c0-112">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="026c0-113">[הפונקציה Func_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) מחפש תוכן התואם את התבנית.</span><span class="sxs-lookup"><span data-stu-id="026c0-113">The [function Func_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span> 
    
  - <span data-ttu-id="026c0-p102">נמצאה מילת מפתח מתוך [Keyword_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) . כולל דוגמאות של מילות מפתח: *לאומי, לאומי #, Soc שניה, מספר תעודת זהות* . לדוגמה, להפעיל דוגמת הבאה עבור המדיניות DLP SSN: **מספר תעודת זהות: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="026c0-p102">A keyword from [Keyword_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found. Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  . For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
    
<span data-ttu-id="026c0-117">לקבלת מידע נוסף אודות מה נדרש עבור SSNs לאתר עבור התוכן שלך, עיין בסעיף הבא במאמר זה: [מה ה רגיש סוגי מידע מחפשים SSNs](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="026c0-117">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="026c0-118">באמצעות סוג אחר מידע רגיש מוכללים, ראה את המאמר הבא לקבלת מידע על מה נדרש עבור סוגים אחרים: [מה ה רגיש סוגי מידע לחפש](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="026c0-118">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

