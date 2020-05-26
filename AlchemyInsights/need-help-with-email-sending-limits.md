---
title: זקוק לעזרה עם מגבלות שליחת דואר אלקטרוני?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357863"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="f147e-102">זקוק לעזרה עם מגבלות שליחת דואר אלקטרוני?</span><span class="sxs-lookup"><span data-stu-id="f147e-102">Need help with email sending limits?</span></span>

<span data-ttu-id="f147e-103">להלן **מגבלות השליחה לפי עיצוב** שנאכפת בשירות.</span><span class="sxs-lookup"><span data-stu-id="f147e-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="f147e-104">מידע נוסף על מגבלות אלה מתועד [כאן](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="f147e-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="f147e-105">כדי להרתיע משלוחים של הודעות בצובר שלא התבקשו, אנו מחילים מגבלות של קצב נמענים לפי משתמש לכל **ההודעות היוצאות והפנימיות**.</span><span class="sxs-lookup"><span data-stu-id="f147e-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="f147e-106">על פני כל SKUs, מגבלה זו היא **10,000 נמענים ליום**.</span><span class="sxs-lookup"><span data-stu-id="f147e-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="f147e-107">לקוחות שצריכים לשלוח דואר אלקטרוני לגיטימי לפרסום בצובר (לדוגמה, ידיעונים של לקוחות) צריכים להשתמש בספקי צד שלישי המתמחים בשירותים אלה.</span><span class="sxs-lookup"><span data-stu-id="f147e-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="f147e-108">**הערה**: לאחר ההגעה למגבלת קצב ההודעות לנמען, לא ניתן לשלוח הודעות מתיבת הדואר עד שמספר הנמענים שנשלחו הודעות ב -24 השעות האחרונות ירד מתחת למגבלה.</span><span class="sxs-lookup"><span data-stu-id="f147e-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="f147e-109">המשתמש לא יוכל לשלוח הודעות עד לנקודה זו.</span><span class="sxs-lookup"><span data-stu-id="f147e-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="f147e-110">מגבלת קצב הודעה של **30 הודעות לדקה** מוחלת על כל ה-skus.</span><span class="sxs-lookup"><span data-stu-id="f147e-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="f147e-111">פעולה זו קובעת את מספר ההודעות שהמשתמש יכול לשלוח מחשבון Exchange Online שלהם בתקופה שצוינה.</span><span class="sxs-lookup"><span data-stu-id="f147e-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="f147e-112">**מספר הנמענים המירבי המותר בשדות אל, עותק ועותק מוסתר** עבור הודעת דואר אלקטרוני בודדת, לאורך כל ה-skus, הוא **1000 נמענים**.</span><span class="sxs-lookup"><span data-stu-id="f147e-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="f147e-113">כדי להתאים אישית מגבלה זו, המשך [לכאן](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="f147e-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
