---
title: אתר מודרני בתור אתר הבסיס
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666871"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="92e3f-102">אתר מודרני כאתר בסיס</span><span class="sxs-lookup"><span data-stu-id="92e3f-102">Modern site as root site</span></span>

<span data-ttu-id="92e3f-103">התחלנו להציג תכונה חדשה שתאפשר לך [להחליף את אתר הבסיס הקלאסי של האתר באמצעות אתר מודרני](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="92e3f-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="92e3f-104">השתמש באפשרות [הפעל את SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) כדי להחליף את המיקום של אתר באתר אחר בזמן אחסון האתר המקורי.</span><span class="sxs-lookup"><span data-stu-id="92e3f-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="92e3f-105">זמין עבור שני אתרי הצוות (שאינם מחוברים לקבוצה) ולאתר תקשורת.</span><span class="sxs-lookup"><span data-stu-id="92e3f-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="92e3f-106">אל תמחק את אתר הבסיס הקלאסי כדי ליצור אתר תקשורת מודרני.</span><span class="sxs-lookup"><span data-stu-id="92e3f-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="92e3f-107">פעולה זו אינה נתמכת על-ידי Microsoft.</span><span class="sxs-lookup"><span data-stu-id="92e3f-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="92e3f-108">מחיקת אתר הבסיס תגרום לכל אתרי SharePoint בארגון שלך לא להיות נגישים לכל המשתמשים, עד שתשחזר את האתר או תיצור אתר חדש באותו כתובת URL.</span><span class="sxs-lookup"><span data-stu-id="92e3f-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="92e3f-109">אנו ניצור תקשורת של תכונה זו דרך מרכז ההודעות.</span><span class="sxs-lookup"><span data-stu-id="92e3f-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="92e3f-110">אתה אמור לצפות שהתכונה מופעלת בדייר שלך בקרוב.</span><span class="sxs-lookup"><span data-stu-id="92e3f-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="92e3f-111">בעיות ידועות בנושא החלפת אתרים</span><span class="sxs-lookup"><span data-stu-id="92e3f-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="92e3f-112">אתר היעד עשוי להחזיר שגיאת "לא נמצא" (HTTP 404) לפרק זמן קצר.</span><span class="sxs-lookup"><span data-stu-id="92e3f-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="92e3f-113">יהיה צורך לסרוק משוב תוכן כדי לעדכן את אינדקס החיפוש.</span><span class="sxs-lookup"><span data-stu-id="92e3f-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="92e3f-114">אין צורך בשלב ידני כאן, פעולה זו תתבצע באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="92e3f-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="92e3f-115">כל דבר תלוי בקישורים סטטיים (כגון קבצי סינכרון וקבצי OneNote) יצטרכו לתקן אותו באופן ידני.</span><span class="sxs-lookup"><span data-stu-id="92e3f-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="92e3f-116">ייתכן שיהיה עליך לאמת את אתרי Project Server כדי לוודא שהם עדיין משויכים כראוי.</span><span class="sxs-lookup"><span data-stu-id="92e3f-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
