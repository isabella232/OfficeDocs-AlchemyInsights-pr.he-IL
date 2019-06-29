---
title: טכנולוגיית DLP כלל עבור לנו מספר חשבון הבנק אינו פועל
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
ms.openlocfilehash: 83050b05cffacd3e81d34f05383c213eb0042fae
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389470"
---
<span data-ttu-id="05c3e-102">האם אתה נתקל בבעיות עם **מניעת אובדן נתונים (DLP)** אינה פועלת עבור תוכן המכיל **מספר חשבון בנק בארה ב** בעת שימוש בסוג מידע רגיש DLP ב- O365?</span><span class="sxs-lookup"><span data-stu-id="05c3e-102">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="05c3e-103">אם כן, ודא כי התוכן שלך מכיל את המידע הדרוש עבור מה המדיניות DLP הוא מחפש כאשר חישובו.</span><span class="sxs-lookup"><span data-stu-id="05c3e-103">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="05c3e-104">לדוגמה, עבור מדיניות **מספר חשבון בנק בארה ב** נקבעה עם רמת הביטחון של 85%, הבאות מוערכים ואת אפשרות לזהות עבור הכלל להפעיל:</span><span class="sxs-lookup"><span data-stu-id="05c3e-104">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="05c3e-105">**[עיצוב:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 ספרות</span><span class="sxs-lookup"><span data-stu-id="05c3e-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="05c3e-106">**[תבנית:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 ספרות עוקבים.</span><span class="sxs-lookup"><span data-stu-id="05c3e-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="05c3e-107">**[בדיקת סיכום:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** לא, קיימת ללא בדיקת סיכום</span><span class="sxs-lookup"><span data-stu-id="05c3e-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="05c3e-108">**[הגדרה:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** מדיניות DLP הוא 75% בטוח כי סוג זה של מידע רגיש זיהה if, בתוך מידת הקירבה של 300 תווים:</span><span class="sxs-lookup"><span data-stu-id="05c3e-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="05c3e-109">הביטוי הרגיל Regex_usa_bank_account_number מוצא תוכן התואם את התבנית</span><span class="sxs-lookup"><span data-stu-id="05c3e-109">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="05c3e-110">נמצאה מילת מפתח מתוך Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="05c3e-110">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="05c3e-111">לדוגמה, להפעיל דוגמת הבאה עבור מדיניות **מספר חשבון בנק בארה ב** : 78344011 חשבון עו ש</span><span class="sxs-lookup"><span data-stu-id="05c3e-111">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="05c3e-112">לקבלת מידע נוסף אודות מה נדרש עבור **מספר חשבון בנק בארה ב** לזהות עבור התוכן שלך, עיין בסעיף הבא במאמר זה: [מה ה רגיש סוגי מידע מחפשים מספר חשבון בנק בארה ב](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="05c3e-112">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="05c3e-113">באמצעות סוג אחר מידע רגיש מוכללים, ראה את המאמר הבא לקבלת מידע על מה נדרש עבור סוגים אחרים: [מה ה רגיש סוגי מידע לחפש](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="05c3e-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  