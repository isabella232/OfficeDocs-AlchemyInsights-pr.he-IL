---
title: זקוק לעזרה עם מגבלות שליחת דואר אלקטרוני?
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
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836280"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="c6df9-102">זקוק לעזרה עם מגבלות שליחת דואר אלקטרוני?</span><span class="sxs-lookup"><span data-stu-id="c6df9-102">Need help with email sending limits?</span></span>

<span data-ttu-id="c6df9-103">להלן **מגבלות השליחה לפי עיצוב** שנאכפות בשירות.</span><span class="sxs-lookup"><span data-stu-id="c6df9-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="c6df9-104">מידע נוסף על מגבלות אלה מתועד [כאן](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="c6df9-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="c6df9-105">כדי להרתיע את המסירה של הודעות בצובר שלא התבקשו, אנו מחילים מגבלות קצב נמען לכל משתמש **על כל ההודעות היוצאות והפניתיות.**</span><span class="sxs-lookup"><span data-stu-id="c6df9-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="c6df9-106">בכל יחידות ה- SK, מגבלה זו היא **10,000 נמענים ליום**.</span><span class="sxs-lookup"><span data-stu-id="c6df9-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="c6df9-107">לקוחות שתצטרך לשלוח דואר אלקטרוני מסחרי מסחרי לגיטימי (לדוגמה, ידיעונים של לקוחות) צריכים להשתמש בספקים של ספקים חיצוני המתמחים בשירותים אלה.</span><span class="sxs-lookup"><span data-stu-id="c6df9-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="c6df9-108">**הערה:** לאחר הגעת מגבלת קצב הנמען, לא ניתן לשלוח הודעות מתיבת הדואר עד למספר הנמענים שנשלחו ב- 24 השעות האחרונות ירידה מתחת למגבלה.</span><span class="sxs-lookup"><span data-stu-id="c6df9-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="c6df9-109">המשתמש לא יוכל לשלוח הודעות עד לנקודה זו.</span><span class="sxs-lookup"><span data-stu-id="c6df9-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="c6df9-110">מגבלת קצב ההודעות **של 30 הודעות** לדקה מוחלת בכל יחידות ה- SK.</span><span class="sxs-lookup"><span data-stu-id="c6df9-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="c6df9-111">פעולה זו קובעת כמה הודעות משתמש יכול לשלוח מחשבון Exchange Online שלו בתוך תקופה שצוינה.</span><span class="sxs-lookup"><span data-stu-id="c6df9-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="c6df9-112">מספר **הנמענים המרבי המותר בשדות אל, עותק** ועותק מוסתר עבור הודעת דואר אלקטרוני בודדת, בכל יחידות ה- SK, הוא **1000 נמענים.**</span><span class="sxs-lookup"><span data-stu-id="c6df9-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="c6df9-113">כדי להתאים אישית מגבלה זו, עבור [לכאן](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="c6df9-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
