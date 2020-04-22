---
title: כלל DLP של מספר כרטיס אשראי שאינו פועל
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 80ff41b3e746f95278ccbf0df19eebb61f7f9ee0
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704202"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="16838-102">DLP בעיות עם מספרי כרטיסי אשראי</span><span class="sxs-lookup"><span data-stu-id="16838-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="16838-103">**חשוב**: בתקופה חסרת תקדים זאת, אנחנו נוקטים בצעדים כדי להבטיח ששירותי SharePoint Online ו- OneDrive יישארו בזמינות גבוהה - לקבלת מידע נוסף, בקר בכתובת[התאמות של תכונה זמנית ב- SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="16838-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="16838-104">**DLP בעיות עם מספרי כרטיסי אשראי**</span><span class="sxs-lookup"><span data-stu-id="16838-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="16838-105">האם אתה נתקל בבעיות **במניעת אובדן נתונים (DLP)** שאינן פועלות עבור תוכן המכיל **מספר כרטיס אשראי** בעת שימוש בסוג מידע רגיש של DLP ב-O365?</span><span class="sxs-lookup"><span data-stu-id="16838-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="16838-106">אם כן, ודא שהתוכן שלך מכיל את המידע הדרוש כדי להפעיל את מדיניות ה-DLP כאשר הוא מוערך.</span><span class="sxs-lookup"><span data-stu-id="16838-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="16838-107">לדוגמה, עבור **מדיניות כרטיס אשראי** שהוגדרה באמצעות רמת ביטחון של 85%, ההערכה הבאה מוערכת ויש לאתרם כדי שהכלל יפעיל:</span><span class="sxs-lookup"><span data-stu-id="16838-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="16838-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 ספרות שניתן לעצב או לא מעוצב (dddddddddd) וחייב לעבור את מבחן luhn.</span><span class="sxs-lookup"><span data-stu-id="16838-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="16838-109">**[תבנית:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** תבנית מורכבת ואיתנה מאוד המזהה קלפים מכל המותגים הגדולים בעולם, כולל ויזה, מאסטרקארד, דיסקקארד, JCB, אמריקן אקספרס, כרטיסי מתנה וכרטיסי סועד.</span><span class="sxs-lookup"><span data-stu-id="16838-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="16838-110">**[בדיקת סיכום:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** כן, בדיקת הסיכום של Luhn</span><span class="sxs-lookup"><span data-stu-id="16838-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="16838-111">**[הגדרה:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** מדיניות DLP היא 85% בטוחה שהיא זיהתה סוג זה של מידע רגיש אם, בסמיכות של 300 תווים:</span><span class="sxs-lookup"><span data-stu-id="16838-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="16838-112">הפונקציה Func_credit_card מאתרת תוכן התואם לתבנית.</span><span class="sxs-lookup"><span data-stu-id="16838-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="16838-113">אחד מהבאים מתקיים:</span><span class="sxs-lookup"><span data-stu-id="16838-113">One of the following is true:</span></span>

  - <span data-ttu-id="16838-114">נמצאה מילת מפתח מKeyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="16838-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="16838-115">נמצאה מילת מפתח מKeyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="16838-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="16838-116">הפונקציה Func_expiration_date מאתרת תאריך בתבנית התאריך המתאימה.</span><span class="sxs-lookup"><span data-stu-id="16838-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="16838-117">בדיקת הסיכום עוברת</span><span class="sxs-lookup"><span data-stu-id="16838-117">The checksum passes</span></span>

    <span data-ttu-id="16838-118">לדוגמה, הדוגמה הבאה תפעיל מדיניות מספר כרטיס אשראי של DLP:</span><span class="sxs-lookup"><span data-stu-id="16838-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="16838-119">ויזה: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="16838-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="16838-120">תאריך תפוגה: 2/2009</span><span class="sxs-lookup"><span data-stu-id="16838-120">Expires: 2/2009</span></span>

<span data-ttu-id="16838-121">לקבלת מידע נוסף אודות הדרוש עבור **מספר כרטיס אשראי** שיזוהה עבור התוכן שלך, עיין בסעיף הבא במאמר זה: [מה סוגי המידע הרגישים מחפשים כרטיס אשראי](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="16838-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="16838-122">באמצעות סוג מידע רגיש ומובנה שונה, עיין במאמר הבא לקבלת מידע אודות הדרוש עבור סוגים אחרים: [מה סוגי המידע הרגישים מחפשים](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="16838-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  