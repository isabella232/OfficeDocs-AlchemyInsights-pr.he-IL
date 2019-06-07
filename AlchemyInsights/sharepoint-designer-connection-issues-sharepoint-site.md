---
title: רמות הרשאה של SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760694"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="f12ef-102">SharePoint Designer בעיות חיבור</span><span class="sxs-lookup"><span data-stu-id="f12ef-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="f12ef-103">אם SharePoint Designer נתקל בבעיות חיבור לאתרי SharePoint, נא נסה את הפתרונות הבאים נפוצים.</span><span class="sxs-lookup"><span data-stu-id="f12ef-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please attempt the following common solutions.</span></span>

<span data-ttu-id="f12ef-104">שלב 1: ודא SharePoint Designer מתעדכן.</span><span class="sxs-lookup"><span data-stu-id="f12ef-104">Step 1: Verify SharePoint Designer is updated.</span></span>

- [<span data-ttu-id="f12ef-105">SharePoint Designer 2013</span><span class="sxs-lookup"><span data-stu-id="f12ef-105">SharePoint Designer 2013</span></span>](https://www.microsoft.com/download/details.aspx?id=35491)

- [<span data-ttu-id="f12ef-106">SharePoint Designer ה-Service Pack 1 (SP1)</span><span class="sxs-lookup"><span data-stu-id="f12ef-106">SharePoint Designer Service Pack 1 (SP1)</span></span>](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [<span data-ttu-id="f12ef-107">עדכון עבור SharePoint Designer 2013 (KB3114721)</span><span class="sxs-lookup"><span data-stu-id="f12ef-107">Update for SharePoint Designer 2013 (KB3114721)</span></span>](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

<span data-ttu-id="f12ef-108">שלב 2: נקה את קבצי מטמון מקומי</span><span class="sxs-lookup"><span data-stu-id="f12ef-108">Step 2: Clear the local cache files</span></span>

- <span data-ttu-id="f12ef-109">סגור את SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="f12ef-109">Close SharePoint Designer 2013.</span></span>

- <span data-ttu-id="f12ef-110">במחשב המקומי, לאתר את התיקיות הבאות כדי להסיר קבצים במטמון.</span><span class="sxs-lookup"><span data-stu-id="f12ef-110">On the local computer, browse to the following folders to remove cached files.</span></span>

- <span data-ttu-id="f12ef-111">לחץ על התחל, הפעלה ומחק כל הקבצים נמצא תחת כל אחד להלן מיקומים.</span><span class="sxs-lookup"><span data-stu-id="f12ef-111">Click Start, Run and delete all files found under each of the below locations.</span></span>

<span data-ttu-id="f12ef-112">שרת %APPDATA%\Microsoft\Web Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="f12ef-112">%APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

<span data-ttu-id="f12ef-113">פתח את SharePoint Designer 2013 והזן את החשבון שוב כדי לראות אם הוא פועל.</span><span class="sxs-lookup"><span data-stu-id="f12ef-113">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="f12ef-114">שלב 3: [להפעיל אימות מודרני עבור 2013 Office בהתקני Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="f12ef-114">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span></span>

<span data-ttu-id="f12ef-115">שלב 4: מנהלים יהיה עליך לאפשר קובץ Script מותאם אישית כדי לאפשר את החיבור SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="f12ef-115">Step 4: Administrators will need to Allow Custom Script to allow the SharePoint Designer connection.</span></span>

<span data-ttu-id="f12ef-116">לקבלת שלבים מפורטים, דוגמאות ושיקולים ראה [אפשר או מנע בקובץ script מותאם אישית](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="f12ef-116">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


