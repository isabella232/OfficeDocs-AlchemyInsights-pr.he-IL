---
title: יצירת אתר SharePoint
ms.author: kirks
author: Techwriter40
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1386"
- "2303"
- "5200004"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 022f572aadae3b4d9f6665f9f8be871d79b51817
ms.sourcegitcommit: f81c56dd4ae7cb2eedc383dd671b9012f3089286
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/19/2019
ms.locfileid: "35802967"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="4c301-102">יצירת אתר SharePoint</span><span class="sxs-lookup"><span data-stu-id="4c301-102">Create a SharePoint site</span></span>

<span data-ttu-id="4c301-103">באפשרותך לראות הבאים לקבלת מידע אודות יצירת אתרים של SharePoint:</span><span class="sxs-lookup"><span data-stu-id="4c301-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="4c301-104">[ניהול אתרים במרכז הניהול של SharePoint חדש](https://docs.microsoft.com/sharepoint/manage-site-creation): למד אודות אפשרויות יצירת אתר, כולל כיצד ליצור אתר קלאסית או אתר צוותים שאינה כוללת קבוצת Office 365.</span><span class="sxs-lookup"><span data-stu-id="4c301-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="4c301-105">[צור אתר צוות ב- SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): למד כיצד ליצור אתר צוות.</span><span class="sxs-lookup"><span data-stu-id="4c301-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Learn how to create a team site.</span></span>
- <span data-ttu-id="4c301-106">[צור אתר תקשורת ב- SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): למד כיצד ליצור אתר תקשורת.</span><span class="sxs-lookup"><span data-stu-id="4c301-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="4c301-107">[ניהול אתרים במרכז הניהול של SharePoint חדש](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): למד כיצד ליצור אתר קלאסית או אתר צוות שאינו כולל קבוצת Office 365.</span><span class="sxs-lookup"><span data-stu-id="4c301-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> [! עצות]
> - <span data-ttu-id="4c301-109">אין אפשרות ליצור אתר עם אותה כתובת URL של אתר קיים.</span><span class="sxs-lookup"><span data-stu-id="4c301-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="4c301-110">אם למחוק אתר המעוניינים להשתמש מחדש של כתובת ה-URL, הוא אפשרי שהאתר שנמחקו עדיין קיימת תחת **אתרים נמחק**.</span><span class="sxs-lookup"><span data-stu-id="4c301-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="4c301-111">כדי לנהל למחוק אתרים, ראה [מחיקת אתר](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="4c301-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="4c301-112">כדי להסיר לחלוטין את אתר עם Powershell, עיין בדוגמה cmdlet [SPSite הסרה](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="4c301-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="4c301-113">ייתכן שמשתמשים מסוימים לא יוכלו ליצור אתר.</span><span class="sxs-lookup"><span data-stu-id="4c301-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="4c301-114">ראה [יצירת אתר ניהול ב- SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="4c301-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="4c301-115">קיימת אפשרות שהאתר מופיע תקוע בזמן **יצירת** זמן רב יותר מהצפוי.</span><span class="sxs-lookup"><span data-stu-id="4c301-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="4c301-116">אם יותר מ- 24 שעות חלפו מאז שראית תחילה את הבעיה, היכנס כרטיס תמיכה.</span><span class="sxs-lookup"><span data-stu-id="4c301-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="4c301-117">במקרים רבים, אנו אתה כבר עובד על פתרון.</span><span class="sxs-lookup"><span data-stu-id="4c301-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="4c301-118">נא תן לנו לפחות 24 שעות להשלמת פתרון.</span><span class="sxs-lookup"><span data-stu-id="4c301-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="4c301-119">אם עליך ליצור אתר צוות חדש שאינו כולל קבוצת Office 365,</span><span class="sxs-lookup"><span data-stu-id="4c301-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


