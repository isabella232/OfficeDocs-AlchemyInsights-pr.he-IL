---
title: בדיקת כתובות העברה בתיבות דואר
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482771"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="beb40-102">בדיקת כתובות העברה בתיבות דואר</span><span class="sxs-lookup"><span data-stu-id="beb40-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="beb40-103">לעתים, האקרים מעבירים את הודעות הדואר האלקטרוני של המשתמשים לעצמם, ולכן תחילה נבדוק לגבי כתובות וכללים להעברה בתיבת הדואר.</span><span class="sxs-lookup"><span data-stu-id="beb40-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="beb40-104">לאחר מכן נבדוק את יומני הביקורת.</span><span class="sxs-lookup"><span data-stu-id="beb40-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="beb40-105">כך ניתן לבדוק כתובות העברה:</span><span class="sxs-lookup"><span data-stu-id="beb40-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="beb40-106">בחר **משתמשים**  >  **פעילים**.</span><span class="sxs-lookup"><span data-stu-id="beb40-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="beb40-107">בחר את המשתמש שהחשבון שלו נחשף.</span><span class="sxs-lookup"><span data-stu-id="beb40-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="beb40-108">בנשלף של שמופיעה, הרחב את **הגדרות הדואר** ולאחר מכן לחץ על **ערוך** **להעברת דואר אלקטרוני**.</span><span class="sxs-lookup"><span data-stu-id="beb40-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="beb40-109">הסר את כתובות ההעברה שאינך מזהה.</span><span class="sxs-lookup"><span data-stu-id="beb40-109">Remove any forwarding addresses you don't recognize.</span></span>