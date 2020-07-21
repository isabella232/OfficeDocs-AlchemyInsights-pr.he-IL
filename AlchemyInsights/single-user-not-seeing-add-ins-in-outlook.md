---
title: משתמש יחיד שאינו רואה תוספות ב-Outlook
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
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197960"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="6a0d6-102">משתמש יחיד שאינו רואה תוספות ב-Outlook</span><span class="sxs-lookup"><span data-stu-id="6a0d6-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="6a0d6-103">המשתמש עשוי להיות חלק מתפקיד שאין לו את הפרמטר Appספורצה המתאים.</span><span class="sxs-lookup"><span data-stu-id="6a0d6-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="6a0d6-104">הפעל יישומון cmdlet זה כדי לברר אם התפקיד הנכון משויך למשתמש:</span><span class="sxs-lookup"><span data-stu-id="6a0d6-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="6a0d6-105">מuser@domain.com-הקצאת משימות-האצלת $false | תבנית-תפקיד אוטומטי של הטבלה, הבעת מבנה השולחן, סוג התור</span><span class="sxs-lookup"><span data-stu-id="6a0d6-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="6a0d6-106">לקבלת מידע נוסף, ראה [ציון מנהלי הרשת והמשתמשים שיכולים להתקין ולנהל תוספות עבור Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="6a0d6-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
