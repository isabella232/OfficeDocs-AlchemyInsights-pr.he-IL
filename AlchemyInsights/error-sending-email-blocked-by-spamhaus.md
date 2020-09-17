---
title: שגיאה בעת שליחת דואר אלקטרוני נחסם על-ידי SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783804"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="3abc3-102">שגיאה בעת שליחת דואר אלקטרוני: מארח לקוח נחסם באמצעות Spamhaus</span><span class="sxs-lookup"><span data-stu-id="3abc3-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="3abc3-103">כתובת ה-IP ששלחה את ההודעה נמצאת ברשימת חסימות הנמצאת בבעלות [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="3abc3-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="3abc3-104">הסיבות לחסימת הSpamhaus כוללות חשבונות שנחשפו, מחשבים שנפרצו שיתוף כתובת IP ציבורית ומדיניות של ספק שירותי אינטרנט (ISP).</span><span class="sxs-lookup"><span data-stu-id="3abc3-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="3abc3-105">תיקונים אפשריים הם:</span><span class="sxs-lookup"><span data-stu-id="3abc3-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="3abc3-106">לקבלת הודעות נכנסות שנחסמו כאשר אתה שולט בשרת הדואר האלקטרוני המשמש כמקור, עליך לקבוע את הסיבה ולהסיר את החסימה מאתר האינטרנט של Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="3abc3-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="3abc3-107">עבור הודעות נכנסות שנחסמו כאשר כתובת ה-IP של המקור שייכת לאדם אחר, בעלי הכתובת צריך להסיר את הבלוק מאתר האינטרנט של Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="3abc3-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="3abc3-108">אם כתובת ה-IP נמצאת ברשימת חסימות המדיניות (PBL), הבעלים יכול להקצות כתובת IP סטטית אחרת או להסיר את הכתובת מ-PBL.</span><span class="sxs-lookup"><span data-stu-id="3abc3-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="3abc3-109">עבור הודעות יוצאות שנחסמו מהתחום שלך המחובר ל-Microsoft, באפשרותך לקבל שגיאה זו אם ההודעות מנותבות באמצעות שירות של צד שלישי.</span><span class="sxs-lookup"><span data-stu-id="3abc3-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="3abc3-110">באפשרותך להשתמש בכלי בדיקת מידע של WHOIS כדי למצוא את הבעלים של כתובת ה-IP החסומה.</span><span class="sxs-lookup"><span data-stu-id="3abc3-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
