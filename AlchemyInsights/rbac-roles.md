---
title: 'תפקידי RBAC '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583546"
---
# <a name="rbac-rules"></a><span data-ttu-id="fcc95-102">כללי RBAC</span><span class="sxs-lookup"><span data-stu-id="fcc95-102">RBAC rules</span></span>

<span data-ttu-id="fcc95-103">אם אתה מקבל את שגיאת ההרשאה:</span><span class="sxs-lookup"><span data-stu-id="fcc95-103">If you get the permission error:</span></span> 

- <span data-ttu-id="fcc95-104">**ללקוח עם מזהה האובייקט אין הרשאה לביצוע פעולות בטווח (קוד: AuthorizationFailed)**: כאשר אתה מנסה ליצור משאב, ודא שאתה מחובר כעת עם משתמש שהוקצה לו הרשאת כתיבה למשאב בטווח שנבחר.</span><span class="sxs-lookup"><span data-stu-id="fcc95-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="fcc95-105">לדוגמה, כדי לנהל מחשבים וירטואליים בקבוצת משאבים, עליך להיות התפקיד ' [משתתף במחשב וירטואלי](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) ' בקבוצה משאבים (או בטווח האב).</span><span class="sxs-lookup"><span data-stu-id="fcc95-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="fcc95-106">לקבלת רשימה של ההרשאות עבור כל תפקיד מוכלל, ראה [תפקידים מוכללים עבור משאבי התכלת](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="fcc95-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="fcc95-107">**אין לך הרשאה ליצור בקשה לתמיכה**: כאשר אתה מנסה ליצור או לעדכן כרטיס תמיכה, ודא שאתה מחובר כעת עם משתמש שהוקצה לו תפקיד בעל הרשאת [התמיכה/](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)SupportTickets/כתיבה של Microsoft.</span><span class="sxs-lookup"><span data-stu-id="fcc95-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="fcc95-108">**לא ניתן ליצור הקצאות תפקידים נוספות (קוד: RoleAssignmentLimitExceeded)**: כאשר אתה מנסה להקצות תפקיד, נסה לצמצם את מספר הקצאות התפקידים על-ידי הקצאת תפקידים לקבוצות במקום זאת.</span><span class="sxs-lookup"><span data-stu-id="fcc95-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="fcc95-109">תכלת תומך עד **2000** הקצאות תפקידים לכל מנוי.</span><span class="sxs-lookup"><span data-stu-id="fcc95-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="fcc95-110">לקבלת פרטים נוספים על תפקידי התכלת RBAC, ראה [תפקידי rbac של התכלת](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="fcc95-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
