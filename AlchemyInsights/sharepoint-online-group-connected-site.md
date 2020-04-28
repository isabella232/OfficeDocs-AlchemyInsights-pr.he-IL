---
title: הוספת קבוצה לאתר SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 8ef33cbd44b01deaf0e45813d019f7696ef5def0
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912967"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="7d4ca-102">בעיות בעת יצירת אתר המחובר לקבוצה ב-SharePoint</span><span class="sxs-lookup"><span data-stu-id="7d4ca-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="7d4ca-103">אירעו מספר בעיות נפוצות בעת יצירה או יצירה מחדש של אתר המחובר לקבוצה.</span><span class="sxs-lookup"><span data-stu-id="7d4ca-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="7d4ca-104">אם מחקת קבוצה והאתר המחובר אליו וברצונך ליצור אתר אחר עם אותה כתובת URL, יהיה עליך להסיר לצמיתות את האתר הקודם.</span><span class="sxs-lookup"><span data-stu-id="7d4ca-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="7d4ca-105">הורד [SPO ניהול מעטפת](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="7d4ca-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="7d4ca-106">לקבלת מידע נוסף על תחילת התחלת עם Powershell, ראה [תחילת התחלת עם מעטפת ניהול מקוונת של SharePoint](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="7d4ca-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="7d4ca-107">הסר את האתר מאתרים שנמחקו באמצעות ה [-Cmdlet Remove-Spodeleאתר](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell.</span><span class="sxs-lookup"><span data-stu-id="7d4ca-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="7d4ca-108">Powershell נדרש כדי למחוק לצמיתות אתרים בקבוצה.</span><span class="sxs-lookup"><span data-stu-id="7d4ca-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="7d4ca-109">אם אתה יוצר אתר מחובר לקבוצה ומקבל אזהרה: **קבוצה אחרת עם אותו כינוי כבר קיימת**, בדוק את הקבוצות הקיימות [ממרכז הניהול של Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="7d4ca-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="7d4ca-110">כדי לפתור את הבעיה, מחק את הקבוצה הקיימת אם אין עוד צורך או צור את האתר עם כינוי אחר שהוקצה.</span><span class="sxs-lookup"><span data-stu-id="7d4ca-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="7d4ca-111">קיימות דרכים שונות ליצירה ולשימוש בקבוצות מודרניות עם SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7d4ca-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="7d4ca-112">באפשרותך לחבר אתרים קיימים לקבוצת Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7d4ca-112">You can connect existing sites to an Microsoft 365 group.</span></span> <span data-ttu-id="7d4ca-113">לקבלת מידע נוסף, ראה [חיבור קבוצת Microsoft 365 באמצעות ממשק המשתמש של SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="7d4ca-113">For more info, see [Connect an Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="7d4ca-114">כדי ליצור אתר המחובר לקבוצת Microsoft 365, יהיה עליך ליצור [אתר צוות](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="7d4ca-114">To create an Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
