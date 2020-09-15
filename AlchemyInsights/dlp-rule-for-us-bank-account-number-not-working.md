---
title: מספר חשבון הבנק של DLP for US אינו פועל
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679297"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="20e9a-102">בעיות ב-DLP עם מספרי חשבון בנק ארה"ב</span><span class="sxs-lookup"><span data-stu-id="20e9a-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="20e9a-103">**חשוב**: בתקופה חסרת תקדים זאת, אנחנו נוקטים בצעדים כדי להבטיח ששירותי SharePoint Online ו- OneDrive יישארו בזמינות גבוהה - לקבלת מידע נוסף, בקר בכתובת[התאמות של תכונה זמנית ב- SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="20e9a-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="20e9a-104">**בעיות ב-DLP עם מספרי חשבון בנק ארה"ב**</span><span class="sxs-lookup"><span data-stu-id="20e9a-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="20e9a-105">האם אתה נתקל בבעיות **במניעת אובדן נתונים (DLP)** לא פועל עבור תוכן המכיל **מספר חשבון בנק אמריקאי** בעת שימוש בסוג מידע רגיש של DLP ב-O365?</span><span class="sxs-lookup"><span data-stu-id="20e9a-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="20e9a-106">אם כן, ודא שהתוכן שלך מכיל את המידע הדרוש עבור הפעולות שבהן מדיניות DLP מחפשת כאשר היא מוערכת.</span><span class="sxs-lookup"><span data-stu-id="20e9a-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="20e9a-107">לדוגמה, עבור מדיניות **מספר חשבון בנק של ארה"ב** המוגדרת עם רמת ביטחון של 85%, הערכים הבאים מוערכים ויש לזהות אותם עבור הכלל לגורם מפעיל:</span><span class="sxs-lookup"><span data-stu-id="20e9a-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="20e9a-108">**[עיצוב:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 ספרות</span><span class="sxs-lookup"><span data-stu-id="20e9a-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="20e9a-109">**[תבנית:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 ספרות רצופות.</span><span class="sxs-lookup"><span data-stu-id="20e9a-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="20e9a-110">**[בדיקת סיכום:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** לא, אין בדיקת סיכום</span><span class="sxs-lookup"><span data-stu-id="20e9a-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="20e9a-111">**[הגדרה:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** מדיניות DLP היא 75% בטוח שהיא זיהתה סוג זה של מידע רגיש אם בתוך סמיכות של 300 תווים:</span><span class="sxs-lookup"><span data-stu-id="20e9a-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="20e9a-112">הביטוי הרגיל Regex_usa_bank_account_number מוצא תוכן שמתאים לתבנית</span><span class="sxs-lookup"><span data-stu-id="20e9a-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="20e9a-113">מילת מפתח מתוך Keyword_usa_Bank_Account מתקיימת.</span><span class="sxs-lookup"><span data-stu-id="20e9a-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="20e9a-114">לדוגמה, הדוגמה הבאה תגרום להפעלת מדיניות **מספר חשבון בנק ארה"ב** : בדיקת חשבון 78344011</span><span class="sxs-lookup"><span data-stu-id="20e9a-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="20e9a-115">לקבלת מידע נוסף אודות הנדרש עבור **מספר חשבון בנק אמריקאי** שיאותר עבור התוכן שלך, עיין בסעיף הבא במאמר זה: [מה סוגי המידע הרגישים מחפשים מספר חשבון בנק בארה](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="20e9a-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="20e9a-116">באמצעות סוג מידע מוכלל אחר שונה, עיין במאמר הבא לקבלת מידע על הדרישות הדרושות עבור סוגים אחרים: [מה סוגי המידע הרגישים מחפשים](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="20e9a-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  