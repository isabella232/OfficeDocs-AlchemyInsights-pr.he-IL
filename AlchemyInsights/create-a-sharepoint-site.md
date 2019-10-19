---
title: יצירת אתר SharePoint
ms.author: efrene
author: efrene
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 30c51d84005534cc1de9e8b8136da1a07be57b73
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36738198"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="59caf-102">יצירת אתר SharePoint</span><span class="sxs-lookup"><span data-stu-id="59caf-102">Create a SharePoint site</span></span>

<span data-ttu-id="59caf-103">באפשרותך לראות את הפרטים הבאים לקבלת מידע אודות יצירת אתר SharePoint:</span><span class="sxs-lookup"><span data-stu-id="59caf-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="59caf-104">[נהל אתרים במרכז הניהול החדש של SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation): למד אודות אפשרויות יצירת אתרים, כולל כיצד ליצור אתר קלאסי או אתר קבוצות שאינו כולל קבוצת Office 365.</span><span class="sxs-lookup"><span data-stu-id="59caf-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="59caf-105">[צור אתר צוות ב-SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): למד כיצד ליצור אתר צוות.</span><span class="sxs-lookup"><span data-stu-id="59caf-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Learn how to create a team site.</span></span>
- <span data-ttu-id="59caf-106">[צור אתר תקשורת ב-SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): למד כיצד ליצור אתר תקשורת.</span><span class="sxs-lookup"><span data-stu-id="59caf-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="59caf-107">[נהל אתרים במרכז הניהול החדש של SharePoint](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): למד כיצד ליצור אתר קלאסי או אתר צוות שאינו כולל קבוצת Office 365.</span><span class="sxs-lookup"><span data-stu-id="59caf-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> <span data-ttu-id="59caf-108">[! טיפים</span><span class="sxs-lookup"><span data-stu-id="59caf-108">[!Tips]</span></span>
> - <span data-ttu-id="59caf-109">אין באפשרותך ליצור אתר עם אותו כתובת URL של אתר קיים.</span><span class="sxs-lookup"><span data-stu-id="59caf-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="59caf-110">אם מחקת אתר והינך מייחל להשתמש שוב בכתובת URL, ייתכן שהאתר שנמחק עדיין קיים תחת **אתרים שנמחקו**.</span><span class="sxs-lookup"><span data-stu-id="59caf-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="59caf-111">כדי לנהל אתרים שנמחקו, [מחק אתר](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="59caf-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="59caf-112">כדי להסיר לחלוטין אתר עם Powershell, עיין בדוגמה ' [הסר-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet '.</span><span class="sxs-lookup"><span data-stu-id="59caf-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="59caf-113">ייתכן שלמשתמשים מסוימים לא תהיה אפשרות ליצור אתר.</span><span class="sxs-lookup"><span data-stu-id="59caf-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="59caf-114">ראה [ניהול יצירת אתרים ב-SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="59caf-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="59caf-115">ייתכן שהאתר נראה תקוע **ביצירת** זמן ארוך מהצפוי.</span><span class="sxs-lookup"><span data-stu-id="59caf-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="59caf-116">אם חלפו יותר מ -24 שעות מאז הפעם הראשונה שראית את הנושא הזה, אנא התחבר כרטיס תמיכה.</span><span class="sxs-lookup"><span data-stu-id="59caf-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="59caf-117">במקרים רבים, אנחנו כבר עובדים על פתרון.</span><span class="sxs-lookup"><span data-stu-id="59caf-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="59caf-118">בבקשה תן לנו לפחות 24. שעות כדי להשלים פיתרון</span><span class="sxs-lookup"><span data-stu-id="59caf-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="59caf-119">אם עליך ליצור אתר צוות חדש שאינו כולל קבוצת Office 365,</span><span class="sxs-lookup"><span data-stu-id="59caf-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


