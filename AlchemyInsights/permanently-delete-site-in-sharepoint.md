---
title: מחק אתר ב- SharePoint לצמיתות
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955169"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="d86c2-102">מחק אתר ב- SharePoint לצמיתות</span><span class="sxs-lookup"><span data-stu-id="d86c2-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="d86c2-103">כדי לעשות שימוש חוזר בכתובת URL מאתר שנמחק (כדי ליצור מחדש אתר), או כדי למחוק לצמיתות אתר מפני שהוא כבר לא בשימוש, באפשרותך להשתמש ב**מחק לצמיתות** ממרכז הניהול החדש של SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d86c2-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="d86c2-104">עבור אל [דף מחיקת אתרים במרכז הניהול החדש של SharePoint](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) והיכנס עם חשבון הכולל הרשאות מנהל מערכת של הארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="d86c2-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="d86c2-105">בעמודה הימנית, בחר אתר.</span><span class="sxs-lookup"><span data-stu-id="d86c2-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="d86c2-106">לחץ על **מחק לצמיתות**.</span><span class="sxs-lookup"><span data-stu-id="d86c2-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="d86c2-107">**הערה**: לא ניתן למחוק לצמיתות אתרים שמחוברים לקבוצה מתוך מרכז הניהול החדש של SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d86c2-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="d86c2-108">במקום זאת, יהיה עליך להשתמש באפשרות[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite).</span><span class="sxs-lookup"><span data-stu-id="d86c2-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="d86c2-109">לקבלת מידע נוסף, ראה [מחק אתר לצמיתות](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="d86c2-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
