---
title: פריסת תוספות עבור יישומי Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/30/2021
ms.locfileid: "52125205"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="3be96-102">פריסת תוספות עבור יישומי Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="3be96-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="3be96-103">פריסה מרכזית היא הדרך המומלצת לפריסת תוספות Office למשתמשים ולקבוצות בארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="3be96-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="3be96-104">כדי לפרוס תוספות, בצע את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="3be96-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="3be96-105">**הערה:** כדי להתקין תוספות עבור Office כמשתמש בודד, ראה [הצגה, ניהול](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)והתקנה של תוספות בתוכניות Office אחרות.</span><span class="sxs-lookup"><span data-stu-id="3be96-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="3be96-106">כמו כן, ודא שרכישה Office של תוספות של חנות Office זמינה.</span><span class="sxs-lookup"><span data-stu-id="3be96-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> 

1. <span data-ttu-id="3be96-107">ודא שהסביבה שלך מותאמת לדרישות לפריסה של תוספות באמצעות פריסה מרכזית.</span><span class="sxs-lookup"><span data-stu-id="3be96-107">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="3be96-108">לקבלת פרטים, [ראה דרישות](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span><span class="sxs-lookup"><span data-stu-id="3be96-108">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="3be96-109">עבור **אל הגדרות**  >    >  **משולבים קבל** אפליקציות במרכז Microsoft 365 כדי לפרוס תוספות.</span><span class="sxs-lookup"><span data-stu-id="3be96-109">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="3be96-110">הערות:</span><span class="sxs-lookup"><span data-stu-id="3be96-110">Notes:</span></span> 

- <span data-ttu-id="3be96-111">אפליקציות משולבות דורשות של למנהל המערכת יש הרשאות מנהל מערכת כללי Exchange מנהל מערכת.</span><span class="sxs-lookup"><span data-stu-id="3be96-111">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="3be96-112">בעת פריסת תוספות למשתמשים מרובים, מומלץ לבצע מטלות באמצעות קבוצות במקום משתמשים בודדים.</span><span class="sxs-lookup"><span data-stu-id="3be96-112">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="3be96-113">לקבלת פרטים, [ראה שיקולים בעת הקצאת תוספת למשתמשים ולקבוצות](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span><span class="sxs-lookup"><span data-stu-id="3be96-113">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="3be96-114">פריסה מרכזית אינה תומכת במשתמשים בקבוצות מקוננות או בקבוצות עם קבוצות אב.</span><span class="sxs-lookup"><span data-stu-id="3be96-114">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="3be96-115">לקבלת פרטים, ראה [מטלות משתמשים וקיבוץ](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span><span class="sxs-lookup"><span data-stu-id="3be96-115">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="3be96-116">ודא ששירות Microsoft 365 App Management (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') זמין עבור משתמשים להיכנס.</span><span class="sxs-lookup"><span data-stu-id="3be96-116">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="3be96-117">לקבלת פרטים, ראה [קביעת תצורה של מאפייני יישום](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span><span class="sxs-lookup"><span data-stu-id="3be96-117">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="3be96-118">אם אתה נתקל בבעיות בפריסת תוספות באמצעות יישומים משולבים, נסה לפרוס [באמצעות תוספות](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span><span class="sxs-lookup"><span data-stu-id="3be96-118">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="3be96-119">לקבלת מידע נוסף, ראה:</span><span class="sxs-lookup"><span data-stu-id="3be96-119">For more information, see:</span></span>

<span data-ttu-id="3be96-120">[פריסת תוספות במרכז הניהול](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [ניהול תוספות במרכז הניהול](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [שימוש ברכיבי ה- cmdlet של PowerShell](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) בפריסה מרכזית לניהול תוספות 
 [פרסום Office תוספות באמצעות פריסה מרכזית דרך מרכז Microsoft 365 הניהול של](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [פתרון בעיות: המשתמש אינו רואה תוספות](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [פתרון בעיות בשגיאות משתמש Office תוספות](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="3be96-120">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>