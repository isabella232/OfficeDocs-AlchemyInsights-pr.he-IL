---
title: החלפת אתר הבסיס הקלאסי באמצעות אתר מודרני
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691180"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="54efa-102">החלפת אתר הבסיס הקלאסי באמצעות אתר מודרני</span><span class="sxs-lookup"><span data-stu-id="54efa-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="54efa-103">אם הסביבה שלך הוגדרה לפני אפריל 2019, באפשרותך לשנות את אתר הבסיס לאתר מודרני באמצעות Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="54efa-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="54efa-104">אם יש לך אתר אחר שבו ברצונך להשתמש כאתר הבסיס שלך, באפשרותך להחליף [(להחליף) את אתר הבסיס](https://docs.microsoft.com/sharepoint/modern-root-site) שלו.</span><span class="sxs-lookup"><span data-stu-id="54efa-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="54efa-105">השתמש באפשרות [הפעל את SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) כדי להחליף את המיקום של אתר באתר אחר בזמן אחסון האתר המקורי.</span><span class="sxs-lookup"><span data-stu-id="54efa-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="54efa-106">זמין עבור שני אתרי הצוות (שאינם מחוברים לקבוצה) ולאתר תקשורת.</span><span class="sxs-lookup"><span data-stu-id="54efa-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="54efa-107">יכולות נוספות יוצגו בקרוב שיאפשרו לך להמשיך להשתמש בתוכן באתר, אך להמיר את האתר הקיים לאתר תקשורת.</span><span class="sxs-lookup"><span data-stu-id="54efa-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="54efa-108">יכולות אלה יסוכמו בהדרגה.</span><span class="sxs-lookup"><span data-stu-id="54efa-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="54efa-109">המשך לבדוק אם קיימים עדכונים במרכז ההודעות.</span><span class="sxs-lookup"><span data-stu-id="54efa-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="54efa-110">בעיות ידועות בנושא החלפת אתרים</span><span class="sxs-lookup"><span data-stu-id="54efa-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="54efa-111">אתר היעד עשוי להחזיר שגיאת "לא נמצא" (HTTP 404) לפרק זמן קצר.</span><span class="sxs-lookup"><span data-stu-id="54efa-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="54efa-112">יהיה צורך לסרוק משוב תוכן כדי לעדכן את אינדקס החיפוש.</span><span class="sxs-lookup"><span data-stu-id="54efa-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="54efa-113">אין צורך בשלב ידני-פעולה זו תתבצע באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="54efa-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="54efa-114">כל דבר תלוי בקישורים סטטיים (כגון קבצי סינכרון וקבצי OneNote) יצטרכו לתקן אותו באופן ידני.</span><span class="sxs-lookup"><span data-stu-id="54efa-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="54efa-115">אם אתר המקור היה אתר חדשות ארגוני, עדכן את כתובת ה-URL.</span><span class="sxs-lookup"><span data-stu-id="54efa-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="54efa-116">קבל רשימה של כל אתרי החדשות הארגוניים.</span><span class="sxs-lookup"><span data-stu-id="54efa-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="54efa-117">ייתכן שיהיה עליך לאמת את אתרי Project Server כדי לוודא שהם עדיין משויכים כראוי.</span><span class="sxs-lookup"><span data-stu-id="54efa-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
