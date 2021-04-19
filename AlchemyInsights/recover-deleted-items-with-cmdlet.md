---
title: שחזור פריטים שנמחקו באמצעות cmdlet
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: d8f2a50f39d7bcd321692ab093e2efa6613e9814
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835812"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="ed0e8-102">שחזור פריטים שנמחקו באמצעות cmdlet</span><span class="sxs-lookup"><span data-stu-id="ed0e8-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="ed0e8-103">השתמש [ב- cmdlet Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) כדי להציג פריטים שנמחקו בתיבות דואר.</span><span class="sxs-lookup"><span data-stu-id="ed0e8-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="ed0e8-104">לאחר שתמצא את הפריטים שנמחקו, השתמש ב- [cmdlet Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) כדי לשחזר אותם.</span><span class="sxs-lookup"><span data-stu-id="ed0e8-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="ed0e8-105">עיין בפרטים [המלאים ב- Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="ed0e8-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="ed0e8-106">יש להקצות לך את התפקיד 'ייצוא ייבוא תיבת דואר' כדי שתוכל להפעיל cmdlet זה.</span><span class="sxs-lookup"><span data-stu-id="ed0e8-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="ed0e8-107">לקבלת מידע [נוסף, ראה Get-RecoverableItems.](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="ed0e8-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
