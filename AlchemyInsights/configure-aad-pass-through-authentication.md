---
title: קביעת תצורה של אימות מעבר של תכלת של Active Directory
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6970"
- "9003915"
ms.openlocfilehash: be993b1f22d89a92afb099937dae815dc9c09e0e
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036296"
---
# <a name="configure-azure-active-directory-pass-through-authentication"></a><span data-ttu-id="29198-102">קביעת תצורה של אימות מעבר של תכלת של Active Directory</span><span class="sxs-lookup"><span data-stu-id="29198-102">Configure Azure Active Directory pass-through authentication</span></span>

<span data-ttu-id="29198-103">להלן כמה מדריכים שיעזרו לך לקבוע את התצורה של אימות מעבר:</span><span class="sxs-lookup"><span data-stu-id="29198-103">Here are some guides to help you configure pass-through authentication:</span></span>

- <span data-ttu-id="29198-104">**כדי להגדיר את החיבור של תכלת Active Directory**: [משתמשי הסינכרון למדריך הכתובות שלך](https://admin.microsoft.com/AdminPortal/Home) מסייעים לך להגדיר סינכרון hash של סיסמאות או אימות מעבר.</span><span class="sxs-lookup"><span data-stu-id="29198-104">**To set up Azure Active Directory Connect**: The [Sync users to your directory](https://admin.microsoft.com/AdminPortal/Home) guide helps you configure password hash synchronization or pass-through authentication.</span></span> <span data-ttu-id="29198-105">תצורה זו מאפשרת למשתמשים להיכנס לדואר האלקטרוני שלהם ואל Active Directory המקומי (בקר תחום) באמצעות אותה סיסמה.</span><span class="sxs-lookup"><span data-stu-id="29198-105">This configuration enables users to sign in to their email and to your on-premises Active Directory (domain controller) using the same password.</span></span>  <span data-ttu-id="29198-106">[משתמשי הסינכרון למדריך הכתובות שלך](https://admin.microsoft.com/AdminPortal/Home) כולל גם כניסה לפדרציה באמצעות שירותי האיחוד של active DIRECTORY (AD FS).</span><span class="sxs-lookup"><span data-stu-id="29198-106">The [Sync users to your directory](https://admin.microsoft.com/AdminPortal/Home) guide also covers federation sign-in with Active Directory Federation Services (AD FS), too.</span></span>

- <span data-ttu-id="29198-107">**כדי להגדיר תכונות של תכלת**: [מדריך ההגדרה של תכלת לספירה מדריך](https://admin.microsoft.com/adminportal/home#/modernonboarding/azureadsetup) אותך באמצעות הגדרת התכונות ב-תכלת Active Directory Basic, כגון ניהול גישה מבוסס קבוצה, איפוס סיסמה בשירות עצמי עבור יישומי ענן, ושרת האפליקציה של מדריכי כתובות של active directory לפרסום יישומי אינטרנט מקומיים.</span><span class="sxs-lookup"><span data-stu-id="29198-107">**To set up Azure features**: The [Azure AD setup guide](https://admin.microsoft.com/adminportal/home#/modernonboarding/azureadsetup) walks you through setting up the features in Azure Active Directory Basic, like group-based access management, self-service password reset for cloud apps, and Azure Active Directory Application Proxy for publishing on-premises web apps.</span></span>


