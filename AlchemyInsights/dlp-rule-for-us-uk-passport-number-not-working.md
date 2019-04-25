---
title: כלל DLP עבור ארה ב / אנגליה מספר דרכון לא עובד
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bb80ef07364a575f6032bb105cff83cd8f95bd63
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404382"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="3d617-102">בעיות עם טכנולוגיית DLP - ארה ב / אנגליה Passport מספרים</span><span class="sxs-lookup"><span data-stu-id="3d617-102">Problems with DLP - US/UK Passport Numbers</span></span>

<span data-ttu-id="3d617-103">האם אתה נתקל בבעיות עם **מניעת אובדן נתונים (DLP)** לא עובד המכיל תוכן **ארה ב / מספר דרכון בבריטניה** בעת שימוש בסוג מידע רגיש DLP ב- O365?</span><span class="sxs-lookup"><span data-stu-id="3d617-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="3d617-104">אם כן, ודא כי התוכן שלך מכיל את המידע הדרוש עבור מה המדיניות DLP הוא מחפש כאשר חישובו.</span><span class="sxs-lookup"><span data-stu-id="3d617-104">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="3d617-105">לדוגמה, עבור **ארה ב / מספר דרכון בבריטניה** מוגדרת עם רמת הביטחון של 75%, הבאות מוערכים והמדיניות אפשרות לזהות עבור כלל להנעת</span><span class="sxs-lookup"><span data-stu-id="3d617-105">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span> 
  
- <span data-ttu-id="3d617-106">**[תבנית:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** תשע ספרות</span><span class="sxs-lookup"><span data-stu-id="3d617-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span> 
    
- <span data-ttu-id="3d617-107">**[תבנית:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** תשע ספרות עוקבים</span><span class="sxs-lookup"><span data-stu-id="3d617-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span> 
    
- <span data-ttu-id="3d617-108">**[בדיקת סיכום:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** לא, קיימת ללא בדיקת סיכום</span><span class="sxs-lookup"><span data-stu-id="3d617-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="3d617-109">**[הגדרה:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** מדיניות DLP הוא 75% בטוח כי סוג זה של מידע רגיש זיהה if, בתוך מידת הקירבה של 300 תווים:</span><span class="sxs-lookup"><span data-stu-id="3d617-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="3d617-110">הפונקציה Func_usa_uk_passport מחפש תוכן התואם את התבנית.</span><span class="sxs-lookup"><span data-stu-id="3d617-110">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="3d617-111">נמצאה מילת מפתח מתוך Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="3d617-111">A keyword from Keyword_passport is found.</span></span>
    
    <span data-ttu-id="3d617-112">לדוגמה, להפעיל דוגמת הבאה עבור **ארה ב / מספר דרכון בבריטניה** מדיניות: מספר דרכון אמריקאי 123456789</span><span class="sxs-lookup"><span data-stu-id="3d617-112">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span> 
    
<span data-ttu-id="3d617-113">לקבלת מידע נוסף אודות מה נדרש עבור ארה ב / אנגליה מספר דרכון לאתר עבור התוכן שלך, עיין בסעיף הבא במאמר זה: [מראה מה ה רגיש סוגי מידע עבור ארצות הברית / מספר דרכון בבריטניה](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="3d617-113">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="3d617-114">באמצעות סוג אחר מידע רגיש מוכללים, ראה את המאמר הבא לקבלת מידע על מה נדרש עבור סוגים אחרים: [מה ה רגיש סוגי מידע לחפש](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="3d617-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

