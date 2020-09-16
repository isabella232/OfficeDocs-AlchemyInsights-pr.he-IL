---
title: הוספת קבוצה לאתר SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771204"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="d8007-102">בעיות בעת יצירת אתר המחובר לקבוצה ב-SharePoint</span><span class="sxs-lookup"><span data-stu-id="d8007-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="d8007-103">מספר בעיות נפוצות נתקלות בעת יצירה או יצירה מחדש של אתר המחובר לקבוצה.</span><span class="sxs-lookup"><span data-stu-id="d8007-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="d8007-104">אם מחקת קבוצה והאתר המחובר שלה וברצונך ליצור אתר אחר עם אותה כתובת URL, יהיה עליך להסיר לצמיתות את האתר הקודם.</span><span class="sxs-lookup"><span data-stu-id="d8007-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="d8007-105">הורד את [מעטפת ניהול SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="d8007-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="d8007-106">לקבלת מידע נוסף אודות תחילת העבודה עם Powershell, ראה תחילת העבודה [עם מעטפת הניהול של SharePoint Online](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="d8007-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="d8007-107">הסר את האתר מאתרים שנמחקו באמצעות ה [-Cmdlet Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell.</span><span class="sxs-lookup"><span data-stu-id="d8007-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="d8007-108">Powershell נדרש כדי למחוק לצמיתות אתרי קבוצה.</span><span class="sxs-lookup"><span data-stu-id="d8007-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="d8007-109">אם אתה יוצר אתר המחובר לקבוצה ומקבל אזהרה: **קבוצה אחרת עם אותה כינוי כבר קיימת**, בדוק את הקבוצות הקיימות מתוך [מרכז הניהול של Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="d8007-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="d8007-110">כדי לפתור את הבעיה, מחק את הקבוצה הקיימת אם היא אינה נחוצה עוד או צור את האתר עם כינוי אחר מוקצה.</span><span class="sxs-lookup"><span data-stu-id="d8007-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="d8007-111">קיימות דרכים שונות ליצור ולהשתמש בקבוצות מודרניות באמצעות SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d8007-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="d8007-112">באפשרותך לחבר אתרים קיימים לקבוצה של Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d8007-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="d8007-113">לקבלת מידע נוסף, ראה [חיבור קבוצה של Microsoft 365 באמצעות ממשק המשתמש של SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="d8007-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="d8007-114">כדי ליצור אתר המחובר לקבוצה של Microsoft 365, יהיה עליך ליצור [אתר צוות](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="d8007-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
