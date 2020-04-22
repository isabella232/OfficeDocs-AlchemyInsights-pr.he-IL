---
title: שגיאה בשליחת דואר אלקטרוני שנחסם על-ידי ספאם
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714259"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="a698d-102">שגיאה בשליחת דואר אלקטרוני: מארח לקוח נחסם באמצעות ספאם</span><span class="sxs-lookup"><span data-stu-id="a698d-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="a698d-103">כתובת ה-IP ששלחה את ההודעה נמצאת ברשימת בלוקים השייכת ל- [ספאם haus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="a698d-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="a698d-104">הסיבות לחסימה של הדואר הזבל כוללות חשבונות פרוצים, מחשבים פרוצים המשתפים כתובת IP ציבורית ומדיניות של ספק שירותי אינטרנט (ISP).</span><span class="sxs-lookup"><span data-stu-id="a698d-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="a698d-105">תיקונים אפשריים הם:</span><span class="sxs-lookup"><span data-stu-id="a698d-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="a698d-106">עבור הודעות נכנסות חסומות שבהן אתה שולט בשרת הדואר האלקטרוני המהווה מקור, עליך לקבוע את הסיבה ולהסיר את הבלוק מאתר האינטרנט של ספאם.</span><span class="sxs-lookup"><span data-stu-id="a698d-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="a698d-107">עבור הודעות נכנסות שנחסמו כאשר כתובת ה-IP המהווה מקור שייכת למישהו אחר, בעלי הכתובת צריך להסיר את הבלוק מאתר האינטרנט של הדואר.</span><span class="sxs-lookup"><span data-stu-id="a698d-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="a698d-108">אם כתובת ה-IP נמצאת ברשימת בלוק המדיניות (PBL), הבעלים יכול להקצות כתובת IP סטטית שונה או להסיר את הכתובת מ-PBL.</span><span class="sxs-lookup"><span data-stu-id="a698d-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="a698d-109">עבור הודעות יוצאות שנחסמו מהתחום שלך המחובר ל-Microsoft, באפשרותך לקבל שגיאה זו אם ההודעות מנותבות באמצעות שירות צד שלישי.</span><span class="sxs-lookup"><span data-stu-id="a698d-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="a698d-110">באפשרותך להשתמש בכלי בדיקת מWHOIS כדי למצוא את הבעלים החסומים של כתובת IP.</span><span class="sxs-lookup"><span data-stu-id="a698d-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
