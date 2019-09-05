---
title: הוספת קבוצה לאתר SharePoint
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750521"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="241be-102">בעיות בעת יצירה או קיבוץ של אתרים מחוברים ב-SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="241be-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="241be-103">אירעו כמה בעיות נפוצות בעת יצירה או יצירה מחדש של אתר המחובר לקבוצה.</span><span class="sxs-lookup"><span data-stu-id="241be-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="241be-104">אם מחקת קבוצה והאתר המחובר אליו וברצונך ליצור אתר אחר עם אותה כתובת URL, יהיה עליך להסיר לצמיתות את האתר הקודם.</span><span class="sxs-lookup"><span data-stu-id="241be-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="241be-105">הורד [SPO ניהול מעטפת](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="241be-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="241be-106">לקבלת מידע נוסף על תחילת התחלת עם powershell, ראה [תחילת התחלת עם מעטפת ניהול מקוונת של SharePoint](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="241be-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="241be-107">הסר את האתר מאתרים שנמחקו באמצעות ה [-Cmdlet Remove-Spodeleאתר](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell.</span><span class="sxs-lookup"><span data-stu-id="241be-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="241be-108">אם אתה יוצר אתר מחובר לקבוצה ומקבל אזהרה קבוצה אחרת עם אותו כינוי כבר קיימת, בדוק את הקבוצות הקיימות מ- [Office 365 ממרכז הניהול](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="241be-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="241be-109">כדי לפתור את הבעיה, מחק את הקבוצה הקיימת אם אין עוד צורך או צור את האתר עם כינוי אחר שהוקצה.</span><span class="sxs-lookup"><span data-stu-id="241be-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="241be-110">קיימות דרכים שונות ליצירה ולשימוש בקבוצות מודרניות עם SharePoint.</span><span class="sxs-lookup"><span data-stu-id="241be-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="241be-111">באפשרותך לחבר אתרים קיימים לקבוצת Office 365.</span><span class="sxs-lookup"><span data-stu-id="241be-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="241be-112">לקבלת מידע נוסף, ראה [חיבור קבוצת Office 365 המשתמשת בפני המשתמש של SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="241be-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="241be-113">כדי ליצור אתר המחובר לקבוצת Office 365, יהיה עליך ליצור אתר צוות.</span><span class="sxs-lookup"><span data-stu-id="241be-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="241be-114">לקבלת מידע נוסף, ראה [יצירת אתר צוות ב-SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="241be-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

