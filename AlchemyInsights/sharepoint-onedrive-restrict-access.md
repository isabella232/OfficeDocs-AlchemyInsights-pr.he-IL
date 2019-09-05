---
title: הגבל גישה ל-SharePoint או OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750665"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="8326e-102">הגבל גישה ל-SharePoint או OneDrive</span><span class="sxs-lookup"><span data-stu-id="8326e-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="8326e-103">קיימות דרכים רבות להגבלת הגישה לשירותי SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8326e-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="8326e-104">שיטות הגבלת גישה שונות אלה מתוארות להלן.</span><span class="sxs-lookup"><span data-stu-id="8326e-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="8326e-105">**הגבלת הרשאה**</span><span class="sxs-lookup"><span data-stu-id="8326e-105">**Permission Restriction**</span></span>

<span data-ttu-id="8326e-106">ב-SharePoint Online ו-OneDrive עבור עסקים, אנו מגבילים גישה לפריטים כגון אתרים, קבצים ותיקיות על-ידי מתן גישה לאותן קבוצות/אנשים שצריכים לגשת אליהם.</span><span class="sxs-lookup"><span data-stu-id="8326e-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="8326e-107">התאמה אישית של הרשאות עבור רשימה או ספריה של SharePoint</span><span class="sxs-lookup"><span data-stu-id="8326e-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="8326e-108">התאמה אישית של הרשאות אתר SharePoint</span><span class="sxs-lookup"><span data-stu-id="8326e-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="8326e-109">שינוי ההרשאות בתיקיית משנה</span><span class="sxs-lookup"><span data-stu-id="8326e-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="8326e-110">בקרת גישה ממכשירים לא מנוהלים</span><span class="sxs-lookup"><span data-stu-id="8326e-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="8326e-111">כמנהל SharePoint או מנהל כללי ב-Office 365, באפשרותך לחסום או להגביל את הגישה לתוכן SharePoint ו-OneDrive מהתקנים לא מנוהלים (אלה שאינם מחוברים ל-AD היברידי או תואמי ב-Intune).</span><span class="sxs-lookup"><span data-stu-id="8326e-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="8326e-112">**הגבלת מיקום רשת**</span><span class="sxs-lookup"><span data-stu-id="8326e-112">**Network Location Restriction**</span></span>

<span data-ttu-id="8326e-113">כמנהל IT, באפשרותך לשלוט בגישה למשאבי SharePoint ו-OneDrive בהתבסס על מיקומי רשת מוגדרים שבהם אתה נותן אמון.</span><span class="sxs-lookup"><span data-stu-id="8326e-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="8326e-114">פעולה זו ידועה גם כמדיניות מבוססת מיקום.</span><span class="sxs-lookup"><span data-stu-id="8326e-114">This is also known as location-based policy.</span></span> <span data-ttu-id="8326e-115">לקבלת מידע נוסף, עיין [בבקרת גישה לנתוני SharePoint Online ו-OneDrive בהתבסס על מיקום הרשת](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="8326e-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="8326e-116">**הגבלת נעילת אתר**</span><span class="sxs-lookup"><span data-stu-id="8326e-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="8326e-117">בתוך SharePoint Online יש לך את היכולת לנעול אוסף אתרים, כך שלאף אחד אין גישה.</span><span class="sxs-lookup"><span data-stu-id="8326e-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="8326e-118">זה מוגדר באמצעות PowerShell ואת [מעטפת ניהול מקוונת של SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) באמצעות המאפיין [set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) מדינה לוקזיט.</span><span class="sxs-lookup"><span data-stu-id="8326e-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="8326e-119">**הגבלת משתמשים מיצירת אתרים או אתרי מאתר**</span><span class="sxs-lookup"><span data-stu-id="8326e-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="8326e-120">כמנהל הכללי של SharePoint admin או Office 365, באפשרותך לאפשר למשתמשים שלך ליצור ולנהל אתרי SharePoint משלהם, לקבוע אילו אתרים הם יכולים ליצור ולציין את מיקום האתרים.</span><span class="sxs-lookup"><span data-stu-id="8326e-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="8326e-121">לקבלת מידע נוסף, עיין [בניהול יצירת אתרים ב-SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="8326e-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

