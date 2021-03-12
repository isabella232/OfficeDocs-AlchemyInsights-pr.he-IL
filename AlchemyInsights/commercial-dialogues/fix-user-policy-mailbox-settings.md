---
title: תיקון הגדרות מדיניות המשתמש/תיבת הדואר
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746728"
---
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="9138d-102">תיקון הגדרות מדיניות המשתמש/תיבת הדואר</span><span class="sxs-lookup"><span data-stu-id="9138d-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="9138d-103">הגדרות ' דואר זבל ' בתיבת הדואר השפיעו על הודעה זו.</span><span class="sxs-lookup"><span data-stu-id="9138d-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="9138d-104">כדי לסקור את ההגדרות, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="9138d-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="9138d-105">הפעל את מעטפת ניהול Exchange.</span><span class="sxs-lookup"><span data-stu-id="9138d-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="9138d-106">לקבלת מידע נוסף, ראה [פתיחת מעטפת ניהול Exchange](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="9138d-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="9138d-107">הפעיל פקודה זו (באמצעות כתובת הדואר האלקטרוני של המשתמש):  **get-mailboxjunkmailconfiguration-identity "user@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="9138d-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="9138d-108">בדוק אם כתובת הדואר האלקטרוני של השולח היא חלק מ- **TrustedSendersAndDomains** או מ- **BlockedSendersAndDomains**.</span><span class="sxs-lookup"><span data-stu-id="9138d-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="9138d-109">אם כתובת הדואר האלקטרוני נמצאת באחת מהרשימות, ייתכן שתצטרך להסיר אותה.</span><span class="sxs-lookup"><span data-stu-id="9138d-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="9138d-110">לקבלת מידע נוסף, ראה [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span><span class="sxs-lookup"><span data-stu-id="9138d-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
