---
title: סינכרון קבוצה
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256796"
---
# <a name="group-sync"></a><span data-ttu-id="840fc-102">סינכרון קבוצה</span><span class="sxs-lookup"><span data-stu-id="840fc-102">Group sync</span></span>

<span data-ttu-id="840fc-103">מאמר זה מספק הנחיות לסינכרון קבוצתי.</span><span class="sxs-lookup"><span data-stu-id="840fc-103">This article provides guidance on group synchronization.</span></span>

1. <span data-ttu-id="840fc-104">אם אין באפשרותו של מנהל מערכת כללי או של בעלים של קבוצה לשנות מאפייני קבוצה או להוסיף חברים או להקצות בעלים בפורטל התכלת, ודא שמקור הסמכות עבור הקבוצה הוא תכלת Active Directory (תכלת לספירה) עבור בעלי הניהול הכללי או הקבוצה כדי לשנות את הקבוצה.</span><span class="sxs-lookup"><span data-stu-id="840fc-104">If a global admin or group owner is not able to modify group properties or add members or assign owners in the Azure portal, ensure the source of the authority for the group is Azure Active Directory (Azure AD) for the global admin or group owner to modify the group.</span></span>
2. <span data-ttu-id="840fc-105">לפני שתנסה למחוק קבוצה מסונכרנת ב-תכלת AD, ודא [שמחקת את כל הרשיונות שהוקצו](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) כדי למנוע שגיאות.</span><span class="sxs-lookup"><span data-stu-id="840fc-105">Before attempting to delete a synced group in Azure AD, ensure you have [deleted all assigned licenses](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) to avoid errors.</span></span>

<span data-ttu-id="840fc-106">להבנת האופן שבו ניתן לסנכרן משתמשים, קבוצות ואנשי קשר, ראה [הסינכרון של תכלת לספירה](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)ועקוב אחר [סינכרון קבוצה מקומית לתכלת באמצעות תכלת ad connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to סינכרון קבוצות של סלסול באמצעות ad Connect.</span><span class="sxs-lookup"><span data-stu-id="840fc-106">For understanding how to sync users, groups and contacts, see [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), and follow [Syncing an on-premises group to Azure using Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to sync on-perm groups using AD connect.</span></span>

<span data-ttu-id="840fc-107">בצע את הפעולות הבאות לפתרון בעיות בנושא מדריך זה [במהלך הסינכרון](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) כדי לפתור שגיאות נפוצות</span><span class="sxs-lookup"><span data-stu-id="840fc-107">Follow this guide [Troubleshooting Errors during synchronization](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) to troubleshoot common errors during synchronization.</span></span>

