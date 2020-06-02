---
title: שחזור פריטים שנמחקו באמצעות יישומון cmdlet
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: 86744d92a44096991079d1da3bdf4e95e58c55b7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493172"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="efb8d-102">שחזור פריטים שנמחקו באמצעות יישומון cmdlet</span><span class="sxs-lookup"><span data-stu-id="efb8d-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="efb8d-103">השתמש ביישומון ה-cmdlet ' [השגת ההתאוששות](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) ' כדי להציג פריטים שנמחקו בתיבות דואר.</span><span class="sxs-lookup"><span data-stu-id="efb8d-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="efb8d-104">לאחר שתמצא את הפריטים שנמחקו, השתמש ביישומון ה [-cmdlet שחזור-החזרת השחזור](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) כדי לשחזרו.</span><span class="sxs-lookup"><span data-stu-id="efb8d-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="efb8d-105">עיין בפרטים המלאים [בפריטים לקבלת ההתאוששות](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="efb8d-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="efb8d-106">אתה צריך להיות מוקצה תפקיד ייבוא תיבת הדואר לפני שתוכל להפעיל יישומון זה.</span><span class="sxs-lookup"><span data-stu-id="efb8d-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="efb8d-107">לקבלת מידע נוסף, עיין [בפריטי ההתאוששות](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) מכאן.</span><span class="sxs-lookup"><span data-stu-id="efb8d-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
