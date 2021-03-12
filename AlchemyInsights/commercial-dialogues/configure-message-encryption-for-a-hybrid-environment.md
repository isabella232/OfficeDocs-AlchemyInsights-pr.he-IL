---
title: קביעת התצורה של הצפנת הודעות עבור סביבה היברידית
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 22c2468b7639680b447b6464431a79b69f7198c3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745401"
---
# <a name="configure-message-encryption-for-a-hybrid-environment"></a><span data-ttu-id="2a5f2-102">קביעת התצורה של הצפנת הודעות עבור סביבה היברידית</span><span class="sxs-lookup"><span data-stu-id="2a5f2-102">Configure message encryption for a hybrid environment</span></span>

<span data-ttu-id="2a5f2-103">עבור סביבות Exchange היברידיות, משתמשים מקומיים יכולים לשלוח דואר אלקטרוני מוצפן באמצעות הצפנת הודעות של Office (בבית) רק אם הדואר האלקטרוני מנותב דרך Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="2a5f2-103">For hybrid Exchange environments, on-premises users can send encrypted email using Office Message Encryption (OME) only if email is routed through Exchange Online.</span></span>

<span data-ttu-id="2a5f2-104">כדי להצפין הודעות דואר אלקטרוני באמצעות גבי, בצע את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="2a5f2-104">To encrypt emails using OME, perform the following steps:</span></span>

1. <span data-ttu-id="2a5f2-105">השתמש [באשף קביעת התצורה ההיברידית](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) כדי להגדיר את הסביבה ההיברידית.</span><span class="sxs-lookup"><span data-stu-id="2a5f2-105">Use the [Hybrid Configuration wizard](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) to set up your hybrid environment.</span></span> <span data-ttu-id="2a5f2-106">אין צורך לבצע שלבים מיוחדים להגדרת הצפנה.</span><span class="sxs-lookup"><span data-stu-id="2a5f2-106">No special steps are required for setting up encryption.</span></span>
2. <span data-ttu-id="2a5f2-107">[הגדר את כללי זרימת הדואר שלך עבור הצפנה](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) כפי שאתה עושה בדרך כלל.</span><span class="sxs-lookup"><span data-stu-id="2a5f2-107">[Set up your mail flow rules for encryption](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) like you normally would.</span></span>


