---
title: משתמשים מרובים שאינם רואים תוספות ב-Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197975"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="94118-102">משתמשים מרובים שאינם רואים תוספות ב-Outlook</span><span class="sxs-lookup"><span data-stu-id="94118-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="94118-103">אם בדקת את התוספות של Outlook ואף אחת מהן אינה מופיעה, כצעד הראשון לפתרון בעיות, השתמש ב **-** cmdlet ' התחבר לארגון ', כדי לבצע שאילתה על הפרמטר _Appספורצה מאופשר_ .</span><span class="sxs-lookup"><span data-stu-id="94118-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="94118-104">אם השאילתה מחזירה ערך של **False**, הגדר פרמטר זה כ- **True** על-ידי שימוש ב **-cmdlet set-config** , כך שתוספות יופיעו כמצופה.</span><span class="sxs-lookup"><span data-stu-id="94118-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="94118-105">לא מומלץ לקבוע כי הפרמטר _Appספורצה מאופשר_ מוגדר כ- **False**.</span><span class="sxs-lookup"><span data-stu-id="94118-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="94118-106">ערך של **שווא** דורס את כל הגדרות התפקיד הניהולי והמשתמש שלעיל ומונע הפעלה של כל היישומים החדשים על-ידי כל משתמש בארגון.</span><span class="sxs-lookup"><span data-stu-id="94118-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="94118-107">לקבלת מידע נוסף, ראה [ציון מנהלי הרשת והמשתמשים שיכולים להתקין ולנהל תוספות עבור Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span><span class="sxs-lookup"><span data-stu-id="94118-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>