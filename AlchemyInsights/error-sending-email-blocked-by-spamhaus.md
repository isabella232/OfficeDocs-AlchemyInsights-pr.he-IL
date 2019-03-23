---
title: שגיאה בשליחת דואר אלקטרוני נחסם על-ידי SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 7d6ad2667613ae948a4abcefafe8d91cf89d2418
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/22/2019
ms.locfileid: "30761634"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="89b56-102">שגיאה בשליחת דואר אלקטרוני: לקוח למארח חסומה באמצעות Spamhaus</span><span class="sxs-lookup"><span data-stu-id="89b56-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="89b56-103">כתובת ה-IP שממנו נשלחה ההודעה נמצא ברשימת החסימות בבעלות [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="89b56-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="89b56-104">סיבות חוסמת Spamhaus לכלול חשבונות פרוץ, שנפרצו מחשבי שיתוף כתובת IP ציבורית ומדיניות ספק שירותי אינטרנט (ISP).</span><span class="sxs-lookup"><span data-stu-id="89b56-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="89b56-105">תיקונים אפשריים הם:</span><span class="sxs-lookup"><span data-stu-id="89b56-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="89b56-106">עבור הודעות נכנסות חסומים שבו אתה שולט שרת דואר אלקטרוני המקור של Office 365, עליך לקבוע את הסיבה ולהסיר את הבלוק מאתר האינטרנט Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="89b56-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>
    
- <span data-ttu-id="89b56-107">עבור הודעות נכנסות חסומים Office 365 שבו כתובת ה-IP של המקור שייך לאדם אחר, הבעלים כתובת צריך להסיר את הבלוק מאתר האינטרנט Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="89b56-107">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="89b56-108">אם כתובת IP היא על רשימת החסימות מדיניות (PBL), הבעלים יכול להקצות כתובת IP סטטית שונים או להסיר את הכתובת ה-PBL.</span><span class="sxs-lookup"><span data-stu-id="89b56-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>
    
- <span data-ttu-id="89b56-109">עבור הודעות יוצאות חסומים מתוך קבוצת המחשבים שלך ב- Office 365, באפשרותך לקבל שגיאה זו אם ההודעות מנותבות דרך שירות צד שלישי.</span><span class="sxs-lookup"><span data-stu-id="89b56-109">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="89b56-110">באפשרותך להשתמש בכלי בדיקת WHOIS כדי למצוא את הבעלים של כתובת IP חסומות.</span><span class="sxs-lookup"><span data-stu-id="89b56-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
    

