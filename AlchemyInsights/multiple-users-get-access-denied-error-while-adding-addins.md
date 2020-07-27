---
title: משתמשים מרובים מקבלים שגיאה ב-Access נדחתה בעת הוספת תוספות ב-Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423714"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="b621e-102">משתמשים מרובים מקבלים שגיאה ב-Access נדחתה בעת הוספת תוספות ב-Outlook</span><span class="sxs-lookup"><span data-stu-id="b621e-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="b621e-103">באפשרותך לציין לאילו מנהלים בארגון שלך יש הרשאות להתקנה ולניהול של תוספות עבור Outlook.</span><span class="sxs-lookup"><span data-stu-id="b621e-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="b621e-104">באפשרותך גם לציין לאילו משתמשים בארגון שלך יש הרשאה להתקין ולנהל תוספות לשימוש שלהם.</span><span class="sxs-lookup"><span data-stu-id="b621e-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="b621e-105">לקבלת פרטים, ראה [ציון המנהלים והמשתמשים שיכולים להתקין ולנהל תוספות עבור Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="b621e-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="b621e-106">כדי לוודא שהקצית בהצלחה הרשאות עבור משתמש, החלף את <Role Name> שם התפקיד לאימות והפעל את הפקודה הבאה ב-Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="b621e-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="b621e-107">תפקיד מקבל <Role Name> -משימות</span><span class="sxs-lookup"><span data-stu-id="b621e-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="b621e-108">דוגמה זו מראה לך כיצד לוודא מי הקצית הרשאות להתקנת תוספות ממאגר Office עבור הארגון.</span><span class="sxs-lookup"><span data-stu-id="b621e-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="b621e-109">PowerShell</span><span class="sxs-lookup"><span data-stu-id="b621e-109">PowerShell</span></span>

<span data-ttu-id="b621e-110">-תפקיד "יישומים ביתיים של ארגון"-משתמשי הגאוטתמשתמשים</span><span class="sxs-lookup"><span data-stu-id="b621e-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="b621e-111">בתוצאות, בדוק את הערכים בעמודת המשתמשים האפקטיביים.</span><span class="sxs-lookup"><span data-stu-id="b621e-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="b621e-112">לקבלת הקצאה מפורטת של תחביר ומידע אודות פרמטרים, ראה [הקצאת משימות לניהול](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="b621e-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 