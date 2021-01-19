---
title: פתרון בעיות בעלים
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7815"
- "9004358"
ms.openlocfilehash: 914d5682a403197a8569bb75fda8a77449f485f6
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901005"
---
# <a name="troubleshoot-owner-issues"></a><span data-ttu-id="617f8-102">פתרון בעיות בעלים</span><span class="sxs-lookup"><span data-stu-id="617f8-102">Troubleshoot owner issues</span></span>

<span data-ttu-id="617f8-103">כדי לפתור בעיות הקשורות לבעלים, בצע את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="617f8-103">To troubleshoot owner-related issues, perform the following steps:</span></span>

1. <span data-ttu-id="617f8-104">[הוסף או שנה מנהלי מנויים של תכלת](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): הקבוצות של תכלת active Directory (תכלת לספירה) נמצאות בבעלות וניהולן על-ידי בעלי קבוצה.</span><span class="sxs-lookup"><span data-stu-id="617f8-104">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure Active Directory (Azure AD) groups are owned and managed by group owners.</span></span> <span data-ttu-id="617f8-105">בעלי קבוצה יכולים להיות משתמשים או מנהלי שירות, והם יכולים לנהל את הקבוצה, כולל חברות.</span><span class="sxs-lookup"><span data-stu-id="617f8-105">Group owners can be users or service principals, and are able to manage the group, including membership.</span></span> <span data-ttu-id="617f8-106">רק בעלי קבוצה או בעלי קבוצה קיימים-ניהול יכולים להקצות בעלים של קבוצה.</span><span class="sxs-lookup"><span data-stu-id="617f8-106">Only existing group owners or group-managing administrators can assign group owners.</span></span> <span data-ttu-id="617f8-107">בעלי קבוצה אינם נדרשים להיות חברים בקבוצה.</span><span class="sxs-lookup"><span data-stu-id="617f8-107">Group owners aren't required to be members of the group.</span></span>
2. <span data-ttu-id="617f8-108">[הוספה או שינוי של מנהלי מנויים של תכלת](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): מאמר זה מתאר כיצד להוסיף או לשנות את תפקיד מנהל המערכת עבור משתמש באמצעות המאמר התכלת RBAC בטווח המנוי.</span><span class="sxs-lookup"><span data-stu-id="617f8-108">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): This article describes how to add or change the administrator role for a user using Azure RBAC at the subscription scope.</span></span>
3. <span data-ttu-id="617f8-109">השתמש ב-PowerShell כדי להוסיף בעלים של קבוצה או בעלים של יישום.</span><span class="sxs-lookup"><span data-stu-id="617f8-109">Use PowerShell to add a group owner or an application owner.</span></span>
