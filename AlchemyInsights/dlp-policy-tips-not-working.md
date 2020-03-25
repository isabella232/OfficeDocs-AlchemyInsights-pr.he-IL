---
title: עצות למדיניות DLP של מדיניות לא פועלות
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932587"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="44a50-102">בעיות עצה של מדיניות DLP</span><span class="sxs-lookup"><span data-stu-id="44a50-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="44a50-103">**חשוב**: לקוחות רבים של SharePoint Online ו-onedrive מנהלים יישומים קריטיים לעסקים נגד השירות המנוהל ברקע.</span><span class="sxs-lookup"><span data-stu-id="44a50-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="44a50-104">אלה כוללים העברת תוכן, מניעת אובדן נתונים (DLP) ופתרונות גיבוי.</span><span class="sxs-lookup"><span data-stu-id="44a50-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="44a50-105">במהלך זמנים חסרי תקדים אלה, אנו נוטלים צעדים כדי להבטיח ששירותי SharePoint Online ו-OneDrive יישארו זמינים ואמינים עבור המשתמשים התלויים בשירות יותר מתמיד בתרחישי עבודה מרוחקים.</span><span class="sxs-lookup"><span data-stu-id="44a50-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="44a50-106">לתמיכה במטרה זו, אנו הטמיעה מגבלות ויסות הדוק יותר על יישומי הרקע (הגירה, DLP ופתרונות גיבוי) בשעות היום של ימי חול.</span><span class="sxs-lookup"><span data-stu-id="44a50-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="44a50-107">אתה צריך לצפות כי יישומים אלה להשיג תפוקה מוגבלת מאוד במהלך הזמנים האלה.</span><span class="sxs-lookup"><span data-stu-id="44a50-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="44a50-108">עם זאת, בשעות הערב ובסוף השבוע של האזור, השירות יהיה מוכן לעבד נפח גבוה יותר באופן משמעותי של בקשות מיישומי רקע.</span><span class="sxs-lookup"><span data-stu-id="44a50-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="44a50-109">**עצות בנוגע למדיניות DLP**</span><span class="sxs-lookup"><span data-stu-id="44a50-109">**DLP policy tips**</span></span>

<span data-ttu-id="44a50-110">בעת שימוש **במדיניות DLP**, משתמשים יכולים לקבל הודעה על הפרת מדיניות עם **תיאורי מדיניות**.</span><span class="sxs-lookup"><span data-stu-id="44a50-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="44a50-111">מנהלים יכולים לקבוע את התצורה של תיאורי מדיניות שיוצגו בעת בדיקת מדיניות ה-DLP שלהם או כאשר המדיניות נמצאת במצב אכיפה מלא.</span><span class="sxs-lookup"><span data-stu-id="44a50-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="44a50-112">כדי לקבוע את התצורה של עצות מדיניות במדיניות DLP שלך במרכז האבטחה והתאימות במצב אכיפה מלאה, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="44a50-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="44a50-113">ודא שעצות המדיניות **הופעלו** בכלל DLP באמצעות השלבים [כאן](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="44a50-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="44a50-114">ודא **שהתוכן שלך תואם** למה **שנדרש** כדי להפעיל את הכלל המתואר במאמר זה [כאן](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="44a50-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="44a50-115">תיאורי מדיניות מוצגים הן ב-OWA והן ב-Outlook.</span><span class="sxs-lookup"><span data-stu-id="44a50-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="44a50-116">עם זאת, בעת שימוש **ב-Outlook 2013 או בגירסה מתקדמת יותר**, עצות המדיניות מוצגות רק בתנאים מסוימים.</span><span class="sxs-lookup"><span data-stu-id="44a50-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="44a50-117">תנאים אלה מפורטים כאן: [תנאים נתמכים עבור Outlook 2013 או גירסה מתקדמת יותר להצגת עצות מדיניות](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="44a50-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="44a50-118">לקבלת מידע נוסף אודות עצות של מדיניות DLP, ראה: [הצגת עצות מדיניות עבור מדיניות dlp](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="44a50-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  