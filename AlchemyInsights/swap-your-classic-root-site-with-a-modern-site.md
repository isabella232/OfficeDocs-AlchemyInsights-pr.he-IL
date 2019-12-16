---
title: החלף את אתר השורש הקלאסי שלך עם אתר מודרני
ms.author: pebaum
author: pebaum
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: fe1f0f662c49de2bd0b5b997697c98309cb7983f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042928"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="1fc76-102">החלף את אתר השורש הקלאסי שלך עם אתר מודרני</span><span class="sxs-lookup"><span data-stu-id="1fc76-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="1fc76-103">אם הסביבה שלך הוגדרה לפני אפריל 2019, באפשרותך לשנות את אתר השורש שלך לאתר מודרני באמצעות Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="1fc76-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="1fc76-104">אם יש לך אתר שונה בו ברצונך להשתמש כאתר הבסיס שלך, באפשרותך להחליף [(להחליף) את אתר השורש](https://docs.microsoft.com/sharepoint/modern-root-site) בו.</span><span class="sxs-lookup"><span data-stu-id="1fc76-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="1fc76-105">השתמש באפשרות [הפעל-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) כדי להחליף את המיקום של אתר באתר אחר בעת אחסון האתר המקורי בארכיון.</span><span class="sxs-lookup"><span data-stu-id="1fc76-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="1fc76-106">זמין עבור האתר הקבוצתי (לא מחובר לקבוצה) ולאתר תקשורת.</span><span class="sxs-lookup"><span data-stu-id="1fc76-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="1fc76-107">יכולות נוספות יוצגו בקרוב שיאפשרו לך להמשיך להשתמש בתוכן באתר, אך להמיר את האתר הקיים לאתר תקשורת.</span><span class="sxs-lookup"><span data-stu-id="1fc76-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="1fc76-108">יכולות אלה יוגלגלו בהדרגה.</span><span class="sxs-lookup"><span data-stu-id="1fc76-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="1fc76-109">המשך לבדוק אם קיימים עדכונים במרכז ההודעות של Office 365.</span><span class="sxs-lookup"><span data-stu-id="1fc76-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="1fc76-110">בעיות ידועות עם החלפת אתרים</span><span class="sxs-lookup"><span data-stu-id="1fc76-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="1fc76-111">אתר היעד עשוי להחזיר שגיאה "לא נמצאה" (HTTP 404) למשך פרק זמן קצר.</span><span class="sxs-lookup"><span data-stu-id="1fc76-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="1fc76-112">התוכן צריך להיות מעודכן כדי לעדכן את אינדקס החיפוש.</span><span class="sxs-lookup"><span data-stu-id="1fc76-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="1fc76-113">אין צורך בצעד ידני-זה ייעשה באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="1fc76-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="1fc76-114">כל דבר התלוי בקישורים "סטטיים" (כגון קבצי סינכרון קבצים ו-OneNote) יהיה צורך לתקן באופן ידני.</span><span class="sxs-lookup"><span data-stu-id="1fc76-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="1fc76-115">אם אתר המקור היה אתר חדשות ארגוני, עדכן את כתובת ה-URL.</span><span class="sxs-lookup"><span data-stu-id="1fc76-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="1fc76-116">תשיגי רשימה של כל. אתרי החדשות האירגוניים</span><span class="sxs-lookup"><span data-stu-id="1fc76-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="1fc76-117">ייתכן שיהיה צורך באימות של אתרי Project Server כדי לוודא שהם עדיין משויכים כראוי.</span><span class="sxs-lookup"><span data-stu-id="1fc76-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





