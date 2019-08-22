---
title: SharePoint Designer בעיות חיבור
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: a4aeaeaea5743c276b907c78317ff30f5610be81
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36508424"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="3f9ed-102">SharePoint Designer בעיות חיבור</span><span class="sxs-lookup"><span data-stu-id="3f9ed-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="3f9ed-103">אם SharePoint Designer נתקל בבעיות חיבור לאתרי SharePoint, נסה את הפתרונות הבאים נפוצים.</span><span class="sxs-lookup"><span data-stu-id="3f9ed-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="3f9ed-104">שלב 1: ודא SharePoint Designer 2013 מתעדכן עם [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) [2 באוגוסט, 2016 עדכון עבור SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="3f9ed-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="3f9ed-105">שלב 2: נקה את קבצי מטמון מקומי:</span><span class="sxs-lookup"><span data-stu-id="3f9ed-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="3f9ed-106">סגור את SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="3f9ed-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="3f9ed-107">במחשב המקומי, הסר את כל הקבצים שנמצאו בכל אחת מהתיקיות הבאות.</span><span class="sxs-lookup"><span data-stu-id="3f9ed-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="3f9ed-108">Extensions\Cache שרת %APPDATA%\Microsoft\Web</span><span class="sxs-lookup"><span data-stu-id="3f9ed-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="3f9ed-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="3f9ed-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="3f9ed-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="3f9ed-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="3f9ed-111">פתח את SharePoint Designer 2013 והזן את החשבון שוב כדי לראות אם הוא פועל.</span><span class="sxs-lookup"><span data-stu-id="3f9ed-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="3f9ed-112">שלב 3: [להפעיל אימות מודרני עבור 2013 Office בהתקני Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="3f9ed-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="3f9ed-113">שלב 4: מנהלים יהיה עליך **לאפשר קובץ Script מותאם אישית** הגדרות מרכז הניהול של SharePoint כדי לאפשר את החיבור SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="3f9ed-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="3f9ed-114">עיין [אפשר או מנע בקובץ script מותאם אישית](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="3f9ed-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


