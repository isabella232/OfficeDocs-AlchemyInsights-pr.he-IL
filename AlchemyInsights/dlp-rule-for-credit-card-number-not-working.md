---
title: טכנולוגיית DLP כלל עבור מספר כרטיס האשראי אינו פועל
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 875afb47175a78c22894720cb0db8222f6f41614
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529956"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="3ac90-102">בעיות מסוג DLP עם מספרי כרטיס אשראי</span><span class="sxs-lookup"><span data-stu-id="3ac90-102">DLP issues with Credit Card Numbers</span></span>

<span data-ttu-id="3ac90-103">האם אתה נתקל בבעיות עם **מניעת אובדן נתונים (DLP)** אינה פועלת עבור תוכן המכיל **מספר כרטיס האשראי** בעת שימוש בסוג מידע רגיש DLP ב- O365?</span><span class="sxs-lookup"><span data-stu-id="3ac90-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="3ac90-104">אם כן, ודא כי התוכן שלך מכיל את המידע הדרוש כדי להפעיל המדיניות DLP כאשר חישובו.</span><span class="sxs-lookup"><span data-stu-id="3ac90-104">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="3ac90-105">לדוגמה, עבור **כרטיס אשראי מדיניות** מוגדרת עם רמת הביטחון של 85%, הבאות מוערכים ואת אפשרות לזהות עבור הכלל להפעיל:</span><span class="sxs-lookup"><span data-stu-id="3ac90-105">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="3ac90-106">**[תבנית:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 ספרות אשר ניתן לעצב או לא מעוצב (dddddddddddddddd) ואת חייבת לעבור מחשב Luhn.</span><span class="sxs-lookup"><span data-stu-id="3ac90-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="3ac90-107">**[תבנית:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** תבנית מורכבים מאוד ולא יציב שמזהה קלפים מתוך כל המותגים העיקריים ברחבי העולם, כולל ויזה, מאסטרקארד, לגלות כרטיס, JCB, אמריקן אקספרס, כרטיסי מתנה, וכרטיסי דיינרס.</span><span class="sxs-lookup"><span data-stu-id="3ac90-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="3ac90-108">**[בדיקת סיכום:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** כן, בדיקת הסיכום Luhn</span><span class="sxs-lookup"><span data-stu-id="3ac90-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="3ac90-109">**[הגדרה:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** מדיניות DLP הוא 85% בטוח כי סוג זה של מידע רגיש זיהה if, בתוך מידת הקירבה של 300 תווים:</span><span class="sxs-lookup"><span data-stu-id="3ac90-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="3ac90-110">הפונקציה Func_credit_card מחפש תוכן התואם את התבנית.</span><span class="sxs-lookup"><span data-stu-id="3ac90-110">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="3ac90-111">אחד מהצעדים הבאים מתקיים:</span><span class="sxs-lookup"><span data-stu-id="3ac90-111">One of the following is true:</span></span>

  - <span data-ttu-id="3ac90-112">נמצאה מילת מפתח מתוך Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="3ac90-112">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="3ac90-113">נמצאה מילת מפתח מתוך Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="3ac90-113">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="3ac90-114">הפונקציה Func_expiration_date מוצא תאריך בתבנית התאריך הנכון.</span><span class="sxs-lookup"><span data-stu-id="3ac90-114">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="3ac90-115">מעביר בדיקת סיכום</span><span class="sxs-lookup"><span data-stu-id="3ac90-115">The checksum passes</span></span>

    <span data-ttu-id="3ac90-116">לדוגמה, דוגמת הבאה יחזיר עבור מדיניות מספר כרטיס אשראי מסוג DLP:</span><span class="sxs-lookup"><span data-stu-id="3ac90-116">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="3ac90-117">ויזה: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="3ac90-117">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="3ac90-118">פג תוקף: 2/2009</span><span class="sxs-lookup"><span data-stu-id="3ac90-118">Expires: 2/2009</span></span>

<span data-ttu-id="3ac90-119">לקבלת מידע נוסף אודות מה נדרש עבור **מספר כרטיס האשראי** לאתר עבור התוכן שלך, עיין בסעיף הבא במאמר זה: [מה ה רגיש סוגי מידע לחפש כרטיס אשראי #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="3ac90-119">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="3ac90-120">באמצעות סוג אחר מידע רגיש מוכללים, ראה את המאמר הבא לקבלת מידע על מה נדרש עבור סוגים אחרים: [מה ה רגיש סוגי מידע לחפש](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="3ac90-120">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  