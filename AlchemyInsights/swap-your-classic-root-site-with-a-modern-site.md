---
title: החלף את אתר הבסיס הקלאסי עם אתר מודרני
ms.author: efrene
author: efrene
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
ms.openlocfilehash: ffb1466fe436d6cab7ae5fdd60c671f5dd2654dd
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36501080"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="65ac3-102">החלף את אתר הבסיס הקלאסי עם אתר מודרני</span><span class="sxs-lookup"><span data-stu-id="65ac3-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="65ac3-103">אם הסביבה שלך הוגדר לפני 2019 באפריל, באפשרותך לשנות את אתר הבסיס שלך לאתר מודרני באמצעות Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="65ac3-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="65ac3-104">אם יש לך אתר אחר שברצונך להשתמש בשם אתר הבסיס שלך, באפשרותך להחליף אתר (swap) הבסיס איתו.</span><span class="sxs-lookup"><span data-stu-id="65ac3-104">If you have a different site that you want to use as your root site, you can replace (swap) the root site with it.</span></span> 
    - <span data-ttu-id="65ac3-105">השתמש [Invoke SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) להחליף את המיקום של אתר עם אתר אחר בעת אחסון בארכיון של האתר המקורי.</span><span class="sxs-lookup"><span data-stu-id="65ac3-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="65ac3-106">אפשרות זו זמינה עבור אתר הצוות (לא מחובר לקבוצה) ואתר תקשורת.</span><span class="sxs-lookup"><span data-stu-id="65ac3-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="65ac3-107">יכולות נוספות שהוכנסו בקרוב אשר יאפשר לך לשמור באמצעות התוכן באתר, אך להמיר אתר קיים לאתר תקשורת.</span><span class="sxs-lookup"><span data-stu-id="65ac3-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="65ac3-108">אלה יכולות לפרוס בהדרגה.</span><span class="sxs-lookup"><span data-stu-id="65ac3-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="65ac3-109">המשך לבדיקת מרכז הודעת Office 365 עבור עדכונים.</span><span class="sxs-lookup"><span data-stu-id="65ac3-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="65ac3-110">בעיות מוכרות עם החלפה של אתרים</span><span class="sxs-lookup"><span data-stu-id="65ac3-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="65ac3-111">אתר היעד עלול להחזיר הודעת שגיאה "לא נמצא" (HTTP 404) עבור פרק זמן קצר.</span><span class="sxs-lookup"><span data-stu-id="65ac3-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="65ac3-112">התוכן יהיה עליך להיות recrawled כדי לעדכן אינדקס החיפוש.</span><span class="sxs-lookup"><span data-stu-id="65ac3-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="65ac3-113">אין לא נדרש שלב ידנית - הדבר יבוצע באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="65ac3-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="65ac3-114">דבר תלוי סטטי"קישורים (כגון קבצי סינכרון קובץ ו- OneNote) יהיה עליך לתקן באופן ידני.</span><span class="sxs-lookup"><span data-stu-id="65ac3-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="65ac3-115">אם אתר המקור היה אתר חדשות של הארגון, לעדכן את כתובת ה-URL.</span><span class="sxs-lookup"><span data-stu-id="65ac3-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="65ac3-116">קבל רשימה של כל אתרי חדשות של הארגון.</span><span class="sxs-lookup"><span data-stu-id="65ac3-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="65ac3-117">אתרים שרת הפרוייקט, ייתכן שתצטרך להיות מאומתים כדי לוודא שהן עדיין משויכת כראוי.</span><span class="sxs-lookup"><span data-stu-id="65ac3-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





