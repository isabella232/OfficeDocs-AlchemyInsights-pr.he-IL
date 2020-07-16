---
title: אודות זהות ביאממר
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148232"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="eecc5-102">אודות זהות ביאממר</span><span class="sxs-lookup"><span data-stu-id="eecc5-102">About identity in Yammer</span></span>

<span data-ttu-id="eecc5-103">מומלץ שכל הרשתות יקחו את השלבים הבאים כדי למנוע בעיות הקשורות לזהויות:</span><span class="sxs-lookup"><span data-stu-id="eecc5-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="eecc5-104">אכוף את הזהות של Office 365 לאחר הקצאת האספקה של Microsoft 365 חשבונות עבור משתמשים בתכלת AD כדי להבטיח שכל המשתמשים יחתמו באמצעות חשבון Microsoft 365 הראשי שלהם.</span><span class="sxs-lookup"><span data-stu-id="eecc5-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="eecc5-105">לקבלת מידע נוסף, ראה [אכיפת זהות Office 365 עבור משתמשי Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="eecc5-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="eecc5-106">אחד רשתות מרובות של יממר.</span><span class="sxs-lookup"><span data-stu-id="eecc5-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="eecc5-107">תצורות מורשת Yammer לאפשר מספר רשתות יממר להיות מחובר דייר אחד.</span><span class="sxs-lookup"><span data-stu-id="eecc5-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="eecc5-108">לקבלת מידע נוסף, ראה [העברת רשת-איחוד רשתות מרובות של יממר](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="eecc5-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="eecc5-109">באופן אופציונלי, אכוף רישוי עבור Yammer כדי לחסום משתמשים מיאממר אם אין להם רישיון.</span><span class="sxs-lookup"><span data-stu-id="eecc5-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="eecc5-110">לקבלת מידע נוסף, ראה [ניהול רשיונות משתמש של Yammer ב-Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="eecc5-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="eecc5-111">לבסוף, בצע ביקורת על רשימת המשתמשים עבור רשתות Yammer ישנות יותר והשהה משתמשים מהדור הקודם.</span><span class="sxs-lookup"><span data-stu-id="eecc5-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="eecc5-112">מומלץ להשהות (לבטל) משתמשים במקום למחוק אותם, מכיוון שמחיקה היא בלתי הפיכה.</span><span class="sxs-lookup"><span data-stu-id="eecc5-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="eecc5-113">לקבלת מידע נוסף, ראה [ביקורת משתמשי Yammer ברשתות המחוברות ל-Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) [והסרת משתמשים](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="eecc5-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="eecc5-114">על-ידי קביעת התצורה של Yammer באמצעות שלבים אלה, תוכל גם להיות מוכן לקבוע את תצורת רשת יאמר עבור מצב מקורי עבור Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="eecc5-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="eecc5-115">לקבלת מידע נוסף, ראה [קביעת תצורה של רשת יאמר עבור מצב מקורי עבור Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="eecc5-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>