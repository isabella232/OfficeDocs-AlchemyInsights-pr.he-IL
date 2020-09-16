---
title: אודות זהות ב-קטרת
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664171"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="ce999-102">אודות זהות ב-קטרת</span><span class="sxs-lookup"><span data-stu-id="ce999-102">About identity in Yammer</span></span>

<span data-ttu-id="ce999-103">מומלץ שכל הרשתות יעברו את השלבים הבאים כדי להימנע מבעיות הקשורות לזהות:</span><span class="sxs-lookup"><span data-stu-id="ce999-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="ce999-104">אכוף את הזהות של Office 365 לאחר הקצאת חשבונות Microsoft 365 עבור משתמשים בתכלת לספירה כדי להבטיח שכל המשתמשים ייכנסו באמצעות חשבון Microsoft 365 הראשי שלהם.</span><span class="sxs-lookup"><span data-stu-id="ce999-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="ce999-105">לקבלת מידע נוסף, ראה [אכיפת זהות של Office 365 עבור משתמשי קטרת](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="ce999-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="ce999-106">איחוד רשתות קטרת מרובות.</span><span class="sxs-lookup"><span data-stu-id="ce999-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="ce999-107">תצורות קטרת מדור קודם מאפשרות הרשאה של רשתות קטרת מרובות לדייר אחד.</span><span class="sxs-lookup"><span data-stu-id="ce999-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="ce999-108">לקבלת מידע נוסף, ראה [העברת רשת-איחוד רשתות קטרת מרובות](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="ce999-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="ce999-109">באופן אופציונלי, אכוף את הרישוי עבור קטרת כדי לחסום משתמשים מ-קטרת אם אין להם רשיון.</span><span class="sxs-lookup"><span data-stu-id="ce999-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="ce999-110">לקבלת מידע נוסף, ראה [ניהול רשיונות משתמשים של קטרת ב-Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="ce999-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="ce999-111">לבסוף, בצע ביקורת על רשימת המשתמשים עבור רשתות קטרת ישנות יותר והשהה משתמשים מדור קודם.</span><span class="sxs-lookup"><span data-stu-id="ce999-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="ce999-112">מומלץ להשעות את המשתמשים (לבטל את ההפעלה) במקום למחוק אותם, מכיוון שמחיקה בלתי הפיכה.</span><span class="sxs-lookup"><span data-stu-id="ce999-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="ce999-113">לקבלת מידע נוסף, ראה [ביקורת של משתמשי קטרת ברשתות המחוברות ל-Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) [והסרת משתמשים](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="ce999-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="ce999-114">על-ידי קביעת התצורה של קטרת באמצעות שלבים אלה, תוכל גם להיות מוכן לקבוע את התצורה של רשת קטרת עבור מצב מקורי של Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ce999-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="ce999-115">לקבלת מידע נוסף, ראה [קביעת תצורה של רשת קטרת עבור מצב מקורי עבור Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="ce999-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>