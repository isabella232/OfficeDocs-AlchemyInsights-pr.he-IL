---
title: כלל DLP של מספר כרטיס אשראי שאינו פועל
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
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932444"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="bbb78-102">DLP בעיות עם מספרי כרטיסי אשראי</span><span class="sxs-lookup"><span data-stu-id="bbb78-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="bbb78-103">**חשוב**: לקוחות רבים של SharePoint Online ו-onedrive מנהלים יישומים קריטיים לעסקים נגד השירות המנוהל ברקע.</span><span class="sxs-lookup"><span data-stu-id="bbb78-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="bbb78-104">אלה כוללים העברת תוכן, מניעת אובדן נתונים (DLP) ופתרונות גיבוי.</span><span class="sxs-lookup"><span data-stu-id="bbb78-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="bbb78-105">במהלך זמנים חסרי תקדים אלה, אנו נוטלים צעדים כדי להבטיח ששירותי SharePoint Online ו-OneDrive יישארו זמינים ואמינים עבור המשתמשים התלויים בשירות יותר מתמיד בתרחישי עבודה מרוחקים.</span><span class="sxs-lookup"><span data-stu-id="bbb78-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="bbb78-106">לתמיכה במטרה זו, אנו הטמיעה מגבלות ויסות הדוק יותר על יישומי הרקע (הגירה, DLP ופתרונות גיבוי) בשעות היום של ימי חול.</span><span class="sxs-lookup"><span data-stu-id="bbb78-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="bbb78-107">אתה צריך לצפות כי יישומים אלה להשיג תפוקה מוגבלת מאוד במהלך הזמנים האלה.</span><span class="sxs-lookup"><span data-stu-id="bbb78-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="bbb78-108">עם זאת, בשעות הערב ובסוף השבוע של האזור, השירות יהיה מוכן לעבד נפח גבוה יותר באופן משמעותי של בקשות מיישומי רקע.</span><span class="sxs-lookup"><span data-stu-id="bbb78-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="bbb78-109">**DLP בעיות עם מספרי כרטיסי אשראי**</span><span class="sxs-lookup"><span data-stu-id="bbb78-109">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="bbb78-110">האם אתה נתקל בבעיות **במניעת אובדן נתונים (DLP)** שאינן פועלות עבור תוכן המכיל **מספר כרטיס אשראי** בעת שימוש בסוג מידע רגיש של DLP ב-O365?</span><span class="sxs-lookup"><span data-stu-id="bbb78-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="bbb78-111">אם כן, ודא שהתוכן שלך מכיל את המידע הדרוש כדי להפעיל את מדיניות ה-DLP כאשר הוא מוערך.</span><span class="sxs-lookup"><span data-stu-id="bbb78-111">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="bbb78-112">לדוגמה, עבור **מדיניות כרטיס אשראי** שהוגדרה באמצעות רמת ביטחון של 85%, ההערכה הבאה מוערכת ויש לאתרם כדי שהכלל יפעיל:</span><span class="sxs-lookup"><span data-stu-id="bbb78-112">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="bbb78-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 ספרות שניתן לעצב או לא מעוצב (dddddddddd) וחייב לעבור את מבחן luhn.</span><span class="sxs-lookup"><span data-stu-id="bbb78-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="bbb78-114">**[תבנית:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** תבנית מורכבת ואיתנה מאוד המזהה קלפים מכל המותגים הגדולים בעולם, כולל ויזה, מאסטרקארד, דיסקקארד, JCB, אמריקן אקספרס, כרטיסי מתנה וכרטיסי סועד.</span><span class="sxs-lookup"><span data-stu-id="bbb78-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="bbb78-115">**[בדיקת סיכום:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** כן, בדיקת הסיכום של Luhn</span><span class="sxs-lookup"><span data-stu-id="bbb78-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="bbb78-116">**[הגדרה:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** מדיניות DLP היא 85% בטוחה שהיא זיהתה סוג זה של מידע רגיש אם, בסמיכות של 300 תווים:</span><span class="sxs-lookup"><span data-stu-id="bbb78-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="bbb78-117">הפונקציה Func_credit_card מאתרת תוכן התואם לתבנית.</span><span class="sxs-lookup"><span data-stu-id="bbb78-117">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="bbb78-118">אחד מהבאים מתקיים:</span><span class="sxs-lookup"><span data-stu-id="bbb78-118">One of the following is true:</span></span>

  - <span data-ttu-id="bbb78-119">נמצאה מילת מפתח מKeyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="bbb78-119">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="bbb78-120">נמצאה מילת מפתח מKeyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="bbb78-120">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="bbb78-121">הפונקציה Func_expiration_date מאתרת תאריך בתבנית התאריך המתאימה.</span><span class="sxs-lookup"><span data-stu-id="bbb78-121">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="bbb78-122">בדיקת הסיכום עוברת</span><span class="sxs-lookup"><span data-stu-id="bbb78-122">The checksum passes</span></span>

    <span data-ttu-id="bbb78-123">לדוגמה, הדוגמה הבאה תפעיל מדיניות מספר כרטיס אשראי של DLP:</span><span class="sxs-lookup"><span data-stu-id="bbb78-123">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="bbb78-124">ויזה: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="bbb78-124">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="bbb78-125">תאריך תפוגה: 2/2009</span><span class="sxs-lookup"><span data-stu-id="bbb78-125">Expires: 2/2009</span></span>

<span data-ttu-id="bbb78-126">לקבלת מידע נוסף אודות הדרוש עבור **מספר כרטיס אשראי** שיזוהה עבור התוכן שלך, עיין בסעיף הבא במאמר זה: [מה סוגי המידע הרגישים מחפשים כרטיס אשראי](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="bbb78-126">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="bbb78-127">באמצעות סוג מידע רגיש ומובנה שונה, עיין במאמר הבא לקבלת מידע אודות הדרוש עבור סוגים אחרים: [מה סוגי המידע הרגישים מחפשים](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="bbb78-127">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  