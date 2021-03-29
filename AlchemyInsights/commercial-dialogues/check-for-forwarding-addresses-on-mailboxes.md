---
title: בדיקת כתובות העברה בתיבות דואר
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403312"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="67c49-102">בדיקת כתובות העברה בתיבות דואר</span><span class="sxs-lookup"><span data-stu-id="67c49-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="67c49-103">לפעמים פורצי מחשבים (האקרים) מעבירים הודעות דואר אלקטרוני של משתמשים לעצמם, ולכן תחילה נבדוק אם קיימים כתובות וכללים להעברה בתיבת הדואר.</span><span class="sxs-lookup"><span data-stu-id="67c49-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="67c49-104">לאחר מכן נבדוק את יומני הביקורת.</span><span class="sxs-lookup"><span data-stu-id="67c49-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="67c49-105">כך ניתן לבדוק אם יש כתובות העברה:</span><span class="sxs-lookup"><span data-stu-id="67c49-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="67c49-106">בחר **משתמשים**  >  **פעילים משתמשים**.</span><span class="sxs-lookup"><span data-stu-id="67c49-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="67c49-107">בחר את המשתמש שהחשבון שלו נחשף לסכנה.</span><span class="sxs-lookup"><span data-stu-id="67c49-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="67c49-108">בתפריט נשלף שמופיע, הרחב את **הגדרות דואר ולאחר** מכן לחץ על ערוך **עבור** העברת **דואר אלקטרוני**.</span><span class="sxs-lookup"><span data-stu-id="67c49-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="67c49-109">הסר את כל כתובות הנמענים שאתה לא מזהה.</span><span class="sxs-lookup"><span data-stu-id="67c49-109">Remove any forwarding addresses you don't recognize.</span></span>