---
title: אתר מודרני כאתר השורש
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2e2bb02b9dbaf7f8ede0b4c5ba8c8f29453309cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054703"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="5a48d-102">אתר מודרני כאתר שורש</span><span class="sxs-lookup"><span data-stu-id="5a48d-102">Modern site as root site</span></span>

<span data-ttu-id="5a48d-103">התחלנו לפריסה תכונה חדשה שתאפשר לך [להחליף את האתר הקלאסי שלך בסיס האתר עם אתר מודרני](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="5a48d-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="5a48d-104">השתמש באפשרות [הפעל-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) כדי להחליף את המיקום של אתר באתר אחר בעת אחסון האתר המקורי בארכיון.</span><span class="sxs-lookup"><span data-stu-id="5a48d-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="5a48d-105">זמין עבור האתר הקבוצתי (לא מחובר לקבוצה) ולאתר תקשורת.</span><span class="sxs-lookup"><span data-stu-id="5a48d-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="5a48d-106">אל תמחק את אתר השורש הקלאסי שלך כדי ליצור אתר תקשורת מודרני.</span><span class="sxs-lookup"><span data-stu-id="5a48d-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="5a48d-107">הדבר אינו נתמך על-ידי Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5a48d-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="5a48d-108">מחיקת אתר הבסיס תהפוך את כל אתרי SharePoint בארגון שלך לנגישים לכל המשתמשים, עד שתשחזר את האתר או תיצור אתר חדש באותו כתובת URL.</span><span class="sxs-lookup"><span data-stu-id="5a48d-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="5a48d-109">אנו מתקשרים עם תכונה זו באמצעות מרכז ההודעות.</span><span class="sxs-lookup"><span data-stu-id="5a48d-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="5a48d-110">אתה צריך לצפות את התכונה להיות מופעלת הדייר שלך בקרוב.</span><span class="sxs-lookup"><span data-stu-id="5a48d-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="5a48d-111">בעיות ידועות עם החלפת אתרים</span><span class="sxs-lookup"><span data-stu-id="5a48d-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="5a48d-112">אתר היעד עשוי להחזיר שגיאה "לא נמצאה" (HTTP 404) למשך פרק זמן קצר.</span><span class="sxs-lookup"><span data-stu-id="5a48d-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="5a48d-113">התוכן צריך להיות מעודכן כדי לעדכן את אינדקס החיפוש.</span><span class="sxs-lookup"><span data-stu-id="5a48d-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="5a48d-114">אין צורך בצעד ידני, זה ייעשה באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="5a48d-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="5a48d-115">כל דבר התלוי בקישורים "סטטיים" (כגון קבצי סינכרון קבצים ו-OneNote) יהיה צורך לתקן באופן ידני.</span><span class="sxs-lookup"><span data-stu-id="5a48d-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="5a48d-116">ייתכן שיהיה צורך באימות של אתרי Project Server כדי לוודא שהם עדיין משויכים כראוי.</span><span class="sxs-lookup"><span data-stu-id="5a48d-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
