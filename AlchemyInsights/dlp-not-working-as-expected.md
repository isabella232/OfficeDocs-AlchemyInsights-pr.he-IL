---
title: DLP לא פועלת כמצופה
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932623"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="5689e-102">DLP לא פועלת כמצופה</span><span class="sxs-lookup"><span data-stu-id="5689e-102">DLP not working as expected</span></span>

<span data-ttu-id="5689e-103">**חשוב**: לקוחות רבים של SharePoint Online ו-onedrive מנהלים יישומים קריטיים לעסקים נגד השירות המנוהל ברקע.</span><span class="sxs-lookup"><span data-stu-id="5689e-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="5689e-104">אלה כוללים העברת תוכן, מניעת אובדן נתונים (DLP) ופתרונות גיבוי.</span><span class="sxs-lookup"><span data-stu-id="5689e-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="5689e-105">במהלך זמנים חסרי תקדים אלה, אנו נוטלים צעדים כדי להבטיח ששירותי SharePoint Online ו-OneDrive יישארו זמינים ואמינים עבור המשתמשים התלויים בשירות יותר מתמיד בתרחישי עבודה מרוחקים.</span><span class="sxs-lookup"><span data-stu-id="5689e-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="5689e-106">לתמיכה במטרה זו, אנו הטמיעה מגבלות ויסות הדוק יותר על יישומי הרקע (הגירה, DLP ופתרונות גיבוי) בשעות היום של ימי חול.</span><span class="sxs-lookup"><span data-stu-id="5689e-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="5689e-107">אתה צריך לצפות כי יישומים אלה להשיג תפוקה מוגבלת מאוד במהלך הזמנים האלה.</span><span class="sxs-lookup"><span data-stu-id="5689e-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="5689e-108">עם זאת, בשעות הערב ובסוף השבוע של האזור, השירות יהיה מוכן לעבד נפח גבוה יותר באופן משמעותי של בקשות מיישומי רקע.</span><span class="sxs-lookup"><span data-stu-id="5689e-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

 <span data-ttu-id="5689e-109">**הגדרת טכנולוגיית DLP**</span><span class="sxs-lookup"><span data-stu-id="5689e-109">**Setting up DLP**</span></span>

<span data-ttu-id="5689e-110">האם אתה נתקל בבעיות עם **מניעת אובדן נתונים (DLP)** ב-Office 365 לא פועל כצפוי?</span><span class="sxs-lookup"><span data-stu-id="5689e-110">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="5689e-111">אם כן, ודא **שמדיניות** ה-dlp שלך מוגדרת כראוי ושהנתונים שלך מכילים את המידע **שמדיניות dlp** מחפשת בעת חישובו.</span><span class="sxs-lookup"><span data-stu-id="5689e-111">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="5689e-112">מדיניות DLP מאפשרת לך לזהות ולהגן על מידע רגיש בארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="5689e-112">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="5689e-113">כדי להגדיר את מדיניות DLP, השתמש במידע [הנמצא כאן](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="5689e-113">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="5689e-114">**מה מדיניות DLP מחפשת**</span><span class="sxs-lookup"><span data-stu-id="5689e-114">**What DLP policies look for**</span></span>
  
<span data-ttu-id="5689e-115">בעת שימוש **בסוגי המידע הרגישים המובנים** במרכז האבטחה והתאימות של Office 365, מדיניות DLP מחפשת תבניות ורכיבים ספציפיים בעת זיהוי סוגים רגישים אלה.</span><span class="sxs-lookup"><span data-stu-id="5689e-115">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="5689e-116">**סוגי מידע רגישים מוכללים**</span><span class="sxs-lookup"><span data-stu-id="5689e-116">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="5689e-117">לקבלת מידע אודות הסוגים המובנים המוכללים ומדיניות DLP מחפשת בעת זיהוי הסוג הרגיש, ראה: [מה מחפשים סוגי המידע הרגישים](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="5689e-117">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="5689e-118">**סוגי מידע רגישים מותאמים אישית**</span><span class="sxs-lookup"><span data-stu-id="5689e-118">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="5689e-119">אם אתה מנסה ליצור סוגי מידע רגישים מותאמים אישית, השתמש במאמר הבא לקבלת מידע אודות אופן יצירת סוג רגיש מותאם אישית: [יצירת סוג מידע רגיש מותאם אישית](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="5689e-119">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="5689e-120">**בדיקת מדיניות DLP**</span><span class="sxs-lookup"><span data-stu-id="5689e-120">**Test a DLP policy**</span></span>

<span data-ttu-id="5689e-121">כדי לבדוק את הנתונים שלך באמצעות סוג מידע מובנה או רגיש מותאם אישית, השתמש באפשרות **סוג מבחן** תחת**סוגי מידע רגישים** **לסיווגים** > .</span><span class="sxs-lookup"><span data-stu-id="5689e-121">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="5689e-122">לקבלת מידע נוסף, ראה [בדיקת סוגי מידע רגישים מותאמים אישית](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="5689e-122">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="5689e-123">**דוחות**</span><span class="sxs-lookup"><span data-stu-id="5689e-123">**Reports**</span></span>
  
- <span data-ttu-id="5689e-124">קבל תובנות מידע רגישות עם [דוחות DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="5689e-124">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="5689e-125">ראה פרטים ספציפיים על האירוע עם [דוח אירוע](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="5689e-125">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
