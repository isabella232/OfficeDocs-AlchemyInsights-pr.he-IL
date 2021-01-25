---
title: תיבת הדואר שלך בארכיון כמעט מלאה
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974404"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="8e0c2-102">תיבת הדואר שלך בארכיון כמעט מלאה</span><span class="sxs-lookup"><span data-stu-id="8e0c2-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="8e0c2-103">אם המשתמש מקבל את האזהרה; **תיבת הדואר שלך בארכיון כמעט מלאה**, או אם עליך להגדיל את תיבת הדואר של הארכיון שלהם, הנה כמה עצות:</span><span class="sxs-lookup"><span data-stu-id="8e0c2-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="8e0c2-104">אם למשתמש הוקצה תוכנית Exchange Online 1, שדרג את הרשיון **לתוכנית Exchange online 2** כדי להגדיל את הגודל מ-50 GB ל-100GB.</span><span class="sxs-lookup"><span data-stu-id="8e0c2-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="8e0c2-105">אם המשתמש כבר מוקצה לאחת מהאפשרויות הבאות: **Exchange Online plan 2** או תוכנית exchange online 1 עם התוספת לאחסון בארכיון של exchange online, השתמש בשלבים שלהלן כדי להפוך אחסון מתרחב אוטומטי לזמין:.</span><span class="sxs-lookup"><span data-stu-id="8e0c2-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="8e0c2-106">[התחבר אל Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="8e0c2-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="8e0c2-107">הפעלת הunifiedgroup הבאים עבור המשתמש:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="8e0c2-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="8e0c2-108">הפעלת הunifiedgroup הבאים כדי לאשר שהוא זמין עבור המשתמש:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="8e0c2-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="8e0c2-109">לקבלת מידע נוסף, ראה:</span><span class="sxs-lookup"><span data-stu-id="8e0c2-109">For more information see:</span></span>

- [<span data-ttu-id="8e0c2-110"> הפיכת אחסון בלתי מוגבל לזמין בארכיון-עזרה למנהלי מערכת-תאימות של Microsoft 365 | Microsoft Docs</span><span class="sxs-lookup"><span data-stu-id="8e0c2-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="8e0c2-111">מגבלות Exchange Online-תיאורי שירותים | Microsoft Docs</span><span class="sxs-lookup"><span data-stu-id="8e0c2-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="8e0c2-112">שדרג לתוכנית עסקית אחרת | Microsoft Docs</span><span class="sxs-lookup"><span data-stu-id="8e0c2-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

