---
title: בעיות חיבור של מעצב SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051714"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="390ac-102">בעיות חיבור של מעצב SharePoint</span><span class="sxs-lookup"><span data-stu-id="390ac-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="390ac-103">אם SharePoint Designer נתקל בבעיות חיבור לאתרי SharePoint, נא נסה את הפתרונות הנפוצים הבאים.</span><span class="sxs-lookup"><span data-stu-id="390ac-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="390ac-104">שלב 1: ודא ש-SharePoint Designer 2013 מתעדכן באמצעות [sharepoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) ו [-2 באוגוסט, 2016 עדכון עבור sharepoint designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="390ac-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="390ac-105">שלב 2: ניקוי קבצי המטמון המקומי:</span><span class="sxs-lookup"><span data-stu-id="390ac-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="390ac-106">סגור את SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="390ac-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="390ac-107">במחשב המקומי, הסר את כל הקבצים שנמצאו בכל אחת מהתיקיות הבאות.</span><span class="sxs-lookup"><span data-stu-id="390ac-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="390ac-108">% Appנתוניםהארכה/הרחבה של שרת אינטרנט \ זיכרון מטמון</span><span class="sxs-lookup"><span data-stu-id="390ac-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="390ac-109">% שגיאת מערכת/מטמון</span><span class="sxs-lookup"><span data-stu-id="390ac-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="390ac-110">% משתמשים ברשת הקבצים האחרים</span><span class="sxs-lookup"><span data-stu-id="390ac-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="390ac-111">פתח את SharePoint Designer 2013 והזן שוב את החשבון כדי לראות אם הוא פועל.</span><span class="sxs-lookup"><span data-stu-id="390ac-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="390ac-112">שלב 3: [הפעלת אימות מודרני עבור Office 2013 בהתקני Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="390ac-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="390ac-113">שלב 4: מנהלי מערכת יצטרכו **לאפשר Script מותאם אישית** בהגדרות מרכז הניהול של sharepoint כדי לאפשר חיבור של מעצב sharepoint.</span><span class="sxs-lookup"><span data-stu-id="390ac-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="390ac-114">ראה [התרה או מניעה של קובץ script מותאם אישית](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="390ac-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


