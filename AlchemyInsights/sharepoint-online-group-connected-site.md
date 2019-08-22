---
title: הוספת קבוצה לאתר SharePoint
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 6aea12d44a44a3e11eaf3fb1bd47ff3e9dbfd9e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507848"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="8f8ed-102">בעיות בעת יצירה או קבוצת אתרים ב- SharePoint Online מחובר</span><span class="sxs-lookup"><span data-stu-id="8f8ed-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="8f8ed-103">ישנן שתי בעיות נפוצות נתקל בעת יצירה או יצירה מחדש של קבוצת האתר מחובר.</span><span class="sxs-lookup"><span data-stu-id="8f8ed-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="8f8ed-104">אם יש למחוק קבוצה ואתר מחובר ואתה מעוניין ליצור אתר אחר עם אותה כתובת URL, יהיה עליך להסיר לצמיתות את האתר הקודם.</span><span class="sxs-lookup"><span data-stu-id="8f8ed-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="8f8ed-105">הורד [מעטפת ניהול SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="8f8ed-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="8f8ed-106">לקבלת מידע נוסף אודות תחילת העבודה עם powershell, ראה [תחילת העבודה עם מעטפת ניהול המקוונת של SharePoint](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="8f8ed-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="8f8ed-107">להסיר את האתר למחוק אתרים באמצעות cmdlet powershell של [SPODeletedSite הסרה](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="8f8ed-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="8f8ed-108">אם יצירת אתר מחובר לקבוצה ולקבל אזהרה שקיימת כבר קבוצה אחרת עם כינוי זהה, בדוק את קבוצות קיימות מתוך [Office 365 ממרכז Admin](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="8f8ed-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="8f8ed-109">כדי לפתור את הבעיה, מחק קבוצה קיימת אם אין עוד צורך או ליצור את האתר עם כינוי אחר שהוקצו.</span><span class="sxs-lookup"><span data-stu-id="8f8ed-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="8f8ed-110">קיימות דרכים שונות כדי ליצור ולהשתמש קבוצות מודרניים עם SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8f8ed-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="8f8ed-111">באפשרותך לחבר אתרים קיימים לקבוצת Office 365.</span><span class="sxs-lookup"><span data-stu-id="8f8ed-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="8f8ed-112">לקבלת מידע נוסף, ראה [התחברות קבוצת Office 365 באמצעות ineterface המשתמש של SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="8f8ed-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="8f8ed-113">כדי ליצור אתר מחובר קבוצה של Office 365, יהיה עליך ליצור אתר צוות.</span><span class="sxs-lookup"><span data-stu-id="8f8ed-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="8f8ed-114">לקבלת מידע נוסף, ראה [יצירת אתר צוות ב- SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="8f8ed-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

