---
title: הגבל גישה ב-SharePoint או ב-OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700456"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="38028-102">הגבל גישה ב-SharePoint או ב-OneDrive</span><span class="sxs-lookup"><span data-stu-id="38028-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="38028-103">קיימות דרכים רבות להגבלת הגישה לשירותי SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="38028-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="38028-104">שיטות הגבלת גישה שונות אלה מחולקות להלן.</span><span class="sxs-lookup"><span data-stu-id="38028-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="38028-105">**הגבלת הרשאה**</span><span class="sxs-lookup"><span data-stu-id="38028-105">**Permission Restriction**</span></span>

<span data-ttu-id="38028-106">ב-SharePoint Online וב-OneDrive for Business, אנו מגבילים את הגישה לפריטים כגון אתרים, קבצים ותיקיות על-ידי הענקת גישה לקבוצות אלה/לאנשים שאמורים לגשת אליהם.</span><span class="sxs-lookup"><span data-stu-id="38028-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="38028-107">התאמה אישית של הרשאות עבור רשימה או ספריה של SharePoint</span><span class="sxs-lookup"><span data-stu-id="38028-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="38028-108">התאמה אישית של הרשאות אתר SharePoint</span><span class="sxs-lookup"><span data-stu-id="38028-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="38028-109">שינוי ההרשאות בתיקיית משנה</span><span class="sxs-lookup"><span data-stu-id="38028-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="38028-110">בקרת גישה ממכשירים לא מנוהלים</span><span class="sxs-lookup"><span data-stu-id="38028-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="38028-111">כמנהל SharePoint או כמנהל מערכת כללי, באפשרותך לחסום או להגביל את הגישה לתוכן של SharePoint ו-OneDrive ממכשירים לא מנוהלים (מודעות לא היברידיות מצורפות או תואמות בתוך המנגינה).</span><span class="sxs-lookup"><span data-stu-id="38028-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="38028-112">**מגבלת מיקום רשת**</span><span class="sxs-lookup"><span data-stu-id="38028-112">**Network Location Restriction**</span></span>

<span data-ttu-id="38028-113">כמנהל IT, באפשרותך לשלוט בגישה למשאבי SharePoint ו-OneDrive בהתבסס על מיקומי רשת מוגדרים שאתה נותן בהם אמון.</span><span class="sxs-lookup"><span data-stu-id="38028-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="38028-114">פעולה זו נקראת גם מדיניות מבוססת מיקום.</span><span class="sxs-lookup"><span data-stu-id="38028-114">This is also known as location-based policy.</span></span> <span data-ttu-id="38028-115">לקבלת מידע נוסף, ראה [שליטה בגישה לנתונים של SharePoint Online ו-OneDrive בהתבסס על מיקום ברשת](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="38028-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="38028-116">**הגבלת נעילת אתר**</span><span class="sxs-lookup"><span data-stu-id="38028-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="38028-117">בתוך SharePoint Online יש לך את היכולת לנעול אוסף אתרים, כך שלאף אחד אין גישה אליו.</span><span class="sxs-lookup"><span data-stu-id="38028-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="38028-118">הגדרה זו מוגדרת באמצעות PowerShell [ומעטפת הניהול של SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) באמצעות המאפיין [set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.</span><span class="sxs-lookup"><span data-stu-id="38028-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="38028-119">**הגבלת משתמשים מיצירת אתרים או אתרי משנה**</span><span class="sxs-lookup"><span data-stu-id="38028-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="38028-120">כמנהל מערכת של SharePoint או כמנהל מערכת כללי, באפשרותך לאפשר למשתמשים ליצור ולנהל אתרי SharePoint משלהם, לקבוע אילו אתרים הם יוכלו ליצור ולציין את מיקום האתרים.</span><span class="sxs-lookup"><span data-stu-id="38028-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="38028-121">לקבלת מידע נוסף, ראה [ניהול יצירת אתרים ב-SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="38028-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

