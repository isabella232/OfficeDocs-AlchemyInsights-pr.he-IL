---
title: ייתכן שטכנולוגיית DLP זקוקה לסוג מותאם אישית
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932659"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="1f97e-102">ייתכן שטכנולוגיית DLP זקוקה לסוג מותאם אישית</span><span class="sxs-lookup"><span data-stu-id="1f97e-102">DLP might need a custom type</span></span>

<span data-ttu-id="1f97e-103">**חשוב**: לקוחות רבים של SharePoint Online ו-onedrive מנהלים יישומים קריטיים לעסקים נגד השירות המנוהל ברקע.</span><span class="sxs-lookup"><span data-stu-id="1f97e-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="1f97e-104">אלה כוללים העברת תוכן, מניעת אובדן נתונים (DLP) ופתרונות גיבוי.</span><span class="sxs-lookup"><span data-stu-id="1f97e-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="1f97e-105">במהלך זמנים חסרי תקדים אלה, אנו נוטלים צעדים כדי להבטיח ששירותי SharePoint Online ו-OneDrive יישארו זמינים ואמינים עבור המשתמשים התלויים בשירות יותר מתמיד בתרחישי עבודה מרוחקים.</span><span class="sxs-lookup"><span data-stu-id="1f97e-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="1f97e-106">לתמיכה במטרה זו, אנו הטמיעה מגבלות ויסות הדוק יותר על יישומי הרקע (הגירה, DLP ופתרונות גיבוי) בשעות היום של ימי חול.</span><span class="sxs-lookup"><span data-stu-id="1f97e-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="1f97e-107">אתה צריך לצפות כי יישומים אלה להשיג תפוקה מוגבלת מאוד במהלך הזמנים האלה.</span><span class="sxs-lookup"><span data-stu-id="1f97e-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="1f97e-108">עם זאת, בשעות הערב ובסוף השבוע של האזור, השירות יהיה מוכן לעבד נפח גבוה יותר באופן משמעותי של בקשות מיישומי רקע.</span><span class="sxs-lookup"><span data-stu-id="1f97e-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="1f97e-109">**טכנולוגיית DLP עשויה לדרוש סוג מידע מותאם אישית**</span><span class="sxs-lookup"><span data-stu-id="1f97e-109">**DLP may require a custom information type**</span></span>

<span data-ttu-id="1f97e-110">באמצעות מדיניות של מניעת אובדן נתונים (DLP), באפשרותך לזהות ולהגן על נתונים רגישים בארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="1f97e-110">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="1f97e-111">בתרחישים מסוימים, ייתכן שיהיה עליך ליצור סוג מידע **מותאם אישית** משלך כדי להגן על הנתונים של הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="1f97e-111">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="1f97e-112">לדוגמה, ייתכן שהארגון שלך יצטרך לזהות ולהגן על מזהי עובדים או על נתונים אחרים בתבנית מסוימת הספציפית לארגון שלך. אם כן, עיין במאמרים הבאים לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="1f97e-112">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="1f97e-113">**התאמה אישית של סוג מידע רגיש מוכלל**</span><span class="sxs-lookup"><span data-stu-id="1f97e-113">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="1f97e-114">אם סוג מידע רגיש מובנה מתאים לצרכיך עם מספר משודרג בלבד, באפשרותך [להתאים אישית סוג מידע רגיש מוכלל](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="1f97e-114">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="1f97e-115">לדוגמה, באפשרותך להוסיף או להסיר מילות מפתח, או להוסיף או להסיר ראיות תומכות כגון תאריך או כתובת.</span><span class="sxs-lookup"><span data-stu-id="1f97e-115">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="1f97e-116">**יצירת סוג מידע רגיש מותאם אישית**</span><span class="sxs-lookup"><span data-stu-id="1f97e-116">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="1f97e-117">אך אם עליך לזהות ולהגן על סוג אחר של מידע רגיש לחלוטין, באפשרותך [ליצור סוג מידע רגיש ומותאם אישית](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) בממשק המשתמש של מרכז התאימות של אבטחה _ אמפר _.</span><span class="sxs-lookup"><span data-stu-id="1f97e-117">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="1f97e-118">**יצירת סוג מידע רגיש מותאם אישית באבטחה _ אמפר _ מרכז התאימות PowerShell**</span><span class="sxs-lookup"><span data-stu-id="1f97e-118">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="1f97e-119">לבסוף, אם ממשק המשתמש אינו מספק את כל האפשרויות הדרושות לך, באפשרותך [ליצור סוג מידע רגיש מותאם אישית באבטחה _ אמפר _ מרכז התאימות PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="1f97e-119">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="1f97e-120">על-ידי התחלה עם קובץ XML, באפשרותך להשתמש בכל אפשרות זמינה.</span><span class="sxs-lookup"><span data-stu-id="1f97e-120">By starting with an XML file, you can use every option available.</span></span>
