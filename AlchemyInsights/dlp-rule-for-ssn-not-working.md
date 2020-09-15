---
title: כלל DLP for SSN אינו פועל
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679370"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="c7480-102">בעיות של DLP עם מספרי תעודת זהות</span><span class="sxs-lookup"><span data-stu-id="c7480-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="c7480-103">**חשוב**: בתקופה חסרת תקדים זאת, אנחנו נוקטים בצעדים כדי להבטיח ששירותי SharePoint Online ו- OneDrive יישארו בזמינות גבוהה - לקבלת מידע נוסף, בקר בכתובת[התאמות של תכונה זמנית ב- SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="c7480-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="c7480-104">**בעיות ב-DLP עם SSNs**</span><span class="sxs-lookup"><span data-stu-id="c7480-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="c7480-105">האם אתה נתקל בבעיות **במניעת אובדן נתונים (DLP)** לא פועל עבור תוכן המכיל **מספר תעודת זהות (SSN)** בעת שימוש בסוג מידע רגיש ב-Microsoft 365?</span><span class="sxs-lookup"><span data-stu-id="c7480-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="c7480-106">אם כן, ודא שהתוכן שלך מכיל את המידע הדרוש עבור מראה מדיניות ה-DLP.</span><span class="sxs-lookup"><span data-stu-id="c7480-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="c7480-107">לדוגמה, עבור מדיניות SSN שתצורתה נקבעה עם רמת בטחון של 85%, הערכים הבאים מוערכים ויש לזהות אותם עבור הכלל לגורם מפעיל:</span><span class="sxs-lookup"><span data-stu-id="c7480-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="c7480-108">**[עיצוב:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 ספרות, שעשויות להופיע בתבנית מעוצבת או לא מעוצבת</span><span class="sxs-lookup"><span data-stu-id="c7480-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="c7480-109">**[תבנית:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** ארבע פונקציות מחפשות SSNs בארבע תבניות שונות:</span><span class="sxs-lookup"><span data-stu-id="c7480-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="c7480-110">Func_ssn מוצא את SSNs עם עיצוב חזק של pre-2011 המעוצב עם מקפים או רווחים (ddd-dd-dddd או ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="c7480-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="c7480-111">Func_unformatted_ssn מוצא את SSNs עם עיצוב חזק של pre-2011 שאינו מעוצב כתשעה ספרות רצופות (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="c7480-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="c7480-112">Func_randomized_formatted_ssn מוצא את post-2011 SSNs המעוצב עם מקפים או רווחים (ddd-dd-dddd או ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="c7480-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="c7480-113">Func_randomized_unformatted_ssn מוצא את post-2011 SSNs שאינם מעוצבים כתשעה ספרות רצופות (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="c7480-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="c7480-114">**[בדיקת סיכום:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** לא, אין בדיקת סיכום</span><span class="sxs-lookup"><span data-stu-id="c7480-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="c7480-115">**[הגדרה:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** מדיניות DLP היא 85% בטוח שהיא זיהתה סוג זה של מידע רגיש אם בתוך סמיכות של 300 תווים:</span><span class="sxs-lookup"><span data-stu-id="c7480-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="c7480-116">[הפונקציה Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) מאתרת תוכן התואם לתבנית.</span><span class="sxs-lookup"><span data-stu-id="c7480-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="c7480-117">מילת מפתח מתוך [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) מתקיימת.</span><span class="sxs-lookup"><span data-stu-id="c7480-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="c7480-118">דוגמאות למילות מפתח כוללות: ביטוח  *לאומי, ביטוח לאומי, Soc שניה, SSN*  .</span><span class="sxs-lookup"><span data-stu-id="c7480-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="c7480-119">לדוגמה, המדגם הבא יגרום להפעלת מדיניות SSN של DLP: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="c7480-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="c7480-120">לקבלת מידע נוסף אודות הנדרש עבור SSNs לצורך זיהוי עבור התוכן שלך, עיין בסעיף הבא במאמר זה: [מה סוגי המידע הרגישים מחפשים את SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="c7480-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="c7480-121">באמצעות סוג מידע מוכלל אחר שונה, עיין במאמר הבא לקבלת מידע על הדרישות הדרושות עבור סוגים אחרים: [מה סוגי המידע הרגישים מחפשים](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="c7480-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  