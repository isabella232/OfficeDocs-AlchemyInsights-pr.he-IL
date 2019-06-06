---
title: הגבל גישה ב- SharePoint או OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 5101366ff65f477c19b9c7f2c0d7065cf88501b0
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735144"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="dd8fe-102">הגבל גישה ב- SharePoint או OneDrive</span><span class="sxs-lookup"><span data-stu-id="dd8fe-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="dd8fe-103">קיימות דרכים רבות כדי להגביל גישה אל שירותי SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="dd8fe-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="dd8fe-104">השיטות השונות של הגבלת גישה המתוארות להלן.</span><span class="sxs-lookup"><span data-stu-id="dd8fe-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="dd8fe-105">הגבלת הרשאה</span><span class="sxs-lookup"><span data-stu-id="dd8fe-105">Permission Restriction</span></span>

<span data-ttu-id="dd8fe-106">ב- SharePoint Online ו OneDrive עבור העסק, אנו להגביל גישה לפריטים כגון אתרים, קבצים ותיקיות על-ידי הענקת גישה אלה הקבוצות/יחידים יש להם גישה בלבד.</span><span class="sxs-lookup"><span data-stu-id="dd8fe-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

[<span data-ttu-id="dd8fe-107">התאמה אישית של הרשאות עבור SharePoint רשימה או ספריה</span><span class="sxs-lookup"><span data-stu-id="dd8fe-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/en-us/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

[<span data-ttu-id="dd8fe-108">להתאים אישית הרשאות באתר SharePoint</span><span class="sxs-lookup"><span data-stu-id="dd8fe-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions)

[<span data-ttu-id="dd8fe-109">לשנות את ההרשאות של תיקיית משנה</span><span class="sxs-lookup"><span data-stu-id="dd8fe-109">Change the permissions on a subfolder</span></span>](https://support.office.com/en-us/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

[<span data-ttu-id="dd8fe-110">בקרת גישה ממכשירים לא מנוהלים</span><span class="sxs-lookup"><span data-stu-id="dd8fe-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/en-us/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="dd8fe-111">SharePoint או מנהל כללי ב- Office 365, באפשרותך לחסום או להגביל את הגישה לתוכן SharePoint ו- OneDrive ממכשירים לא מנוהל (אלה לא היברידית AD המצורפים או תואם ב- Intune).</span><span class="sxs-lookup"><span data-stu-id="dd8fe-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="dd8fe-112">הגבלת מיקום רשת</span><span class="sxs-lookup"><span data-stu-id="dd8fe-112">Network Location Restriction</span></span>

<span data-ttu-id="dd8fe-113">כמנהל IT, תוכל לשלוט בגישה למשאבי SharePoint ו- OneDrive בהתבסס על מיקומי הרשת המוגדרות שאתה נותן בהם אמון.</span><span class="sxs-lookup"><span data-stu-id="dd8fe-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="dd8fe-114">פעולה זו מכונה גם מדיניות המבוססת על מיקום.</span><span class="sxs-lookup"><span data-stu-id="dd8fe-114">This is also known as location-based policy.</span></span> <span data-ttu-id="dd8fe-115">לקבלת מידע נוסף, נא עיין [בקרה על גישה מקוונת של SharePoint ונתונים OneDrive בהתבסס על מיקום הרשת](https://docs.microsoft.com/en-us/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="dd8fe-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/en-us/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="dd8fe-116">הגבלת נעילה של האתר</span><span class="sxs-lookup"><span data-stu-id="dd8fe-116">Site Lock Restriction</span></span> 

<span data-ttu-id="dd8fe-117">בתוך SharePoint Online לך את היכולת לנעול אוסף אתרים, כך שאף אחד יש גישה.</span><span class="sxs-lookup"><span data-stu-id="dd8fe-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="dd8fe-118">מאפיין זה מוגדר באמצעות PowerShell [SharePoint מעטפת ניהול מקוון](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) באמצעות המאפיין [ערכת-SPOSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState.</span><span class="sxs-lookup"><span data-stu-id="dd8fe-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="dd8fe-119">הגבל משתמשים ליצור אתרים או אתרי משנה</span><span class="sxs-lookup"><span data-stu-id="dd8fe-119">Restrict users from creating sites or subsites</span></span>

<span data-ttu-id="dd8fe-120">הניהול של SharePoint או הניהול הכללי של Office 365, באפשרותך לאפשר למשתמשים ליצור, לנהל אתרי SharePoint משלהם, לקבוע איזה סוג של אתרים שהם יכולים ליצור, וציין את מיקום האתרים.</span><span class="sxs-lookup"><span data-stu-id="dd8fe-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="dd8fe-121">לקבלת מידע נוסף, ראה [יצירת אתר ניהול ב- SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="dd8fe-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/manage-site-creation)</span></span>

