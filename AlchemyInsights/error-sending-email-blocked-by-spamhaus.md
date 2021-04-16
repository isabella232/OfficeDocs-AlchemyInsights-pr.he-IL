---
title: שגיאה בשליחת דואר אלקטרוני שנחסם על-ידי SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813725"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="a70a5-102">שגיאה בשליחת דואר אלקטרוני: מארח הלקוח נחסם באמצעות Spamhaus</span><span class="sxs-lookup"><span data-stu-id="a70a5-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="a70a5-103">כתובת ה- IP ששלחה את ההודעה נמצאת ברשימת חסימות בבעלות [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="a70a5-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="a70a5-104">הסיבות לחסומים על-ידי Spamhaus כוללות חשבונות שנפגמו, מחשבים שנפגמו בסכנה החולקים כתובת IP ציבורית ומדיניות ספק שירותי אינטרנט (ISP).</span><span class="sxs-lookup"><span data-stu-id="a70a5-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="a70a5-105">תיקונים אפשריים הם:</span><span class="sxs-lookup"><span data-stu-id="a70a5-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="a70a5-106">עבור הודעות נכנסות חסומות במקום שבו אתה שולט בשרת הדואר האלקטרוני המשמש כמקור, עליך לקבוע את הגורם ולהסיר את הבלוק מהאתר של Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="a70a5-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="a70a5-107">עבור הודעות נכנסות חסומות שייכות לכתובת ה- IP המשמשת כמקור למישהו אחר, בעל הכתובת צריך להסיר את הבלוק מהאתר של Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="a70a5-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="a70a5-108">אם כתובת ה- IP נמצאת ברשימת בלוקי המדיניות (PBL), הבעלים יכול להקצות כתובת IP סטטית אחרת או להסיר את הכתובת מה- PBL.</span><span class="sxs-lookup"><span data-stu-id="a70a5-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="a70a5-109">עבור הודעות יוצאות חסומות מהתחום המחובר ל- Microsoft, באפשרותך לקבל שגיאה זו אם ההודעות מנותב דרך שירות של ספקים שלישיים.</span><span class="sxs-lookup"><span data-stu-id="a70a5-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="a70a5-110">באפשרותך להשתמש בכלי בדיקת מידע של WHOIS כדי למצוא את הבעלים של כתובת ה- IP החסומים.</span><span class="sxs-lookup"><span data-stu-id="a70a5-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
