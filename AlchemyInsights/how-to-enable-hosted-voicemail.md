---
title: כיצד להפוך דואר קולי מתארח לזמין
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/09/2020
ms.locfileid: "49678000"
---
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="717ff-102">כיצד להפוך דואר קולי מתארח לזמין</span><span class="sxs-lookup"><span data-stu-id="717ff-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="717ff-103">כדי להפוך את הדואר הקולי לזמין, **HostedVoicemail** חייב להיות מוגדר ל$true.</span><span class="sxs-lookup"><span data-stu-id="717ff-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="717ff-104">המאפיין **HostedVoicemail** במשתמש שמשתמש ב-PowerShell מרוחק (RPS).</span><span class="sxs-lookup"><span data-stu-id="717ff-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="717ff-105">לקבלת מידע נוסף אודות התחברות ל-RPS, ראה [מבט כולל על Microsoft teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) לקבלת מידע נוסף אודות התחברות ל-RPS.</span><span class="sxs-lookup"><span data-stu-id="717ff-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="717ff-106">מנהל הצוותים אמור להיות מחובר ל-PowerShell מרוחק עבור Teams.</span><span class="sxs-lookup"><span data-stu-id="717ff-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="717ff-107">מ-PowerShell הצג בקשה למנהל הצוותים להפעיל את **set-csuser user@contoso.com-HostedVoiceMail $true** שבו המשתמש של sip הוא המשתמש הנדון.</span><span class="sxs-lookup"><span data-stu-id="717ff-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="717ff-108">שינויים בפריטי מדיניות יכולים להימשך עד 24 שעות כדי לשכפל.</span><span class="sxs-lookup"><span data-stu-id="717ff-108">Changes to policies can take up to 24 hours to replicate.</span></span>