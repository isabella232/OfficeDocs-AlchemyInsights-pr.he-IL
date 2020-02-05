---
title: יצירת אתר SharePoint
ms.author: pebaum
author: todmccoy
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: e1e71ae9401448ed18058f6307302dcbaf773649
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770856"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="7876c-102">יצירת אתר SharePoint</span><span class="sxs-lookup"><span data-stu-id="7876c-102">Create a SharePoint site</span></span>

<span data-ttu-id="7876c-103">צור או נהל אתרים [מאתרים פעילים](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) במרכז הניהול של SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7876c-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="7876c-104">לקבלת מידע נוסף, ראה [ניהול אתרים במרכז הניהול החדש של SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="7876c-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="7876c-105">טיפים</span><span class="sxs-lookup"><span data-stu-id="7876c-105">Tips:</span></span>

- <span data-ttu-id="7876c-106">**אין באפשרותך ליצור** אתר עם אותה כתובת URL של אתר קיים.</span><span class="sxs-lookup"><span data-stu-id="7876c-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="7876c-107">אם מחקת אתר והינך מייחל להשתמש שוב בכתובת URL, ייתכן שהאתר שנמחק עדיין קיים תחת [אתרים שנמחקו](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="7876c-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="7876c-108">יהיה צורך למחוק את האתר לצמיתות כדי להשתמש שוב בכתובת ה-URL.</span><span class="sxs-lookup"><span data-stu-id="7876c-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="7876c-109">כדי להסיר לחלוטין אתר עם Powershell, עיין בדוגמה ' [הסר-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet '.</span><span class="sxs-lookup"><span data-stu-id="7876c-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="7876c-110">ייתכן שלמשתמשים מסוימים לא תהיה אפשרות ליצור אתר.</span><span class="sxs-lookup"><span data-stu-id="7876c-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="7876c-111">[ראה ניהול יצירת אתרים ב-SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="7876c-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="7876c-112">ייתכן שהאתר נראה תקוע **ביצירת** זמן ארוך מהצפוי.</span><span class="sxs-lookup"><span data-stu-id="7876c-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="7876c-113">אם חלפו יותר מ -24 שעות מאז הפעם הראשונה שראית את הנושא הזה, אנא התחבר כרטיס תמיכה.</span><span class="sxs-lookup"><span data-stu-id="7876c-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="7876c-114">במקרים רבים, אנחנו כבר עובדים על פתרון.</span><span class="sxs-lookup"><span data-stu-id="7876c-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="7876c-115">בבקשה תן לנו לפחות 24. שעות כדי להשלים פיתרון</span><span class="sxs-lookup"><span data-stu-id="7876c-115">Please give us at least 24 hours to complete a solution.</span></span>
