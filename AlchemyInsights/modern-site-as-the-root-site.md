---
title: אתר מודרניים כמו אתר הבסיס
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 260048db6c439183da8e0bb0c2dfa3c7475fca79
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/09/2019
ms.locfileid: "36269377"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="b4927-102">אתר מודרני כאתר הבסיס</span><span class="sxs-lookup"><span data-stu-id="b4927-102">Modern site as root site</span></span>

<span data-ttu-id="b4927-103">אנו שהתחילו כדי ההשקה תכונה חדשה שתאפשר לך להחליף את אתר הבסיס אתר קלאסי עם אתר מודרני.</span><span class="sxs-lookup"><span data-stu-id="b4927-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="b4927-104">השתמש [Invoke SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) להחליף את המיקום של אתר עם אתר אחר בעת אחסון בארכיון של האתר המקורי.</span><span class="sxs-lookup"><span data-stu-id="b4927-104">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="b4927-105">אפשרות זו זמינה עבור אתר הצוות (לא מחובר לקבוצה) ואתר תקשורת.</span><span class="sxs-lookup"><span data-stu-id="b4927-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="b4927-106">אל תמחק את אתר הבסיס קלאסית ליצירת אתר תקשורת מודרניים.</span><span class="sxs-lookup"><span data-stu-id="b4927-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="b4927-107">פעולה זו אינה נתמכת על-ידי Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b4927-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="b4927-108">מחיקת אתר הבסיס יבצע כל אתרי SharePoint בארגון שלך נגישים לכל המשתמשים, עד לשחזר את האתר או ליצור אתר חדש בכתובת ה-URL זהה.</span><span class="sxs-lookup"><span data-stu-id="b4927-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="b4927-109">אנו לקיים תקשורת תכונה זו דרך מרכז ההודעה.</span><span class="sxs-lookup"><span data-stu-id="b4927-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="b4927-110">עליך לצפות את התכונה כדי להיות מופעלת בדיירים שלך בקרוב.</span><span class="sxs-lookup"><span data-stu-id="b4927-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="b4927-111">בעיות מוכרות עם החלפה של אתרים</span><span class="sxs-lookup"><span data-stu-id="b4927-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="b4927-112">אתר היעד עלול להחזיר הודעת שגיאה "לא נמצא" (HTTP 404) עבור פרק זמן קצר.</span><span class="sxs-lookup"><span data-stu-id="b4927-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="b4927-113">התוכן יהיה עליך להיות recrawled כדי לעדכן אינדקס החיפוש.</span><span class="sxs-lookup"><span data-stu-id="b4927-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="b4927-114">אין שלב ידני לא נדרש כאן, הדבר יבוצע באופן אוטומטי.</span><span class="sxs-lookup"><span data-stu-id="b4927-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="b4927-115">דבר תלוי סטטי"קישורים (כגון קבצי סינכרון קובץ ו- OneNote) יהיה עליך לתקן באופן ידני.</span><span class="sxs-lookup"><span data-stu-id="b4927-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="b4927-116">אתרים שרת הפרוייקט, ייתכן שתצטרך להיות מאומתים כדי לוודא שהן עדיין משויכת כראוי.</span><span class="sxs-lookup"><span data-stu-id="b4927-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
