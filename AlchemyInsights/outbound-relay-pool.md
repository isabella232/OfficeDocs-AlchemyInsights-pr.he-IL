---
title: מאגר ממסר יוצא
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381715"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="a9635-102">מאגר ממסר יוצא</span><span class="sxs-lookup"><span data-stu-id="a9635-102">Outbound relay pool</span></span>

<span data-ttu-id="a9635-103">Microsoft גורמת לשינויים מסוימים בתצורה עבור העברה או העברה של דואר אלקטרוני באמצעות Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a9635-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="a9635-104">הודעות בתרחישים מסוימים מועברות או מועברות דרך Microsoft 365 באמצעות מאגר ממסר מיוחד.</span><span class="sxs-lookup"><span data-stu-id="a9635-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="a9635-105">הודעות הנשלחות באמצעות מאגר הממסר עלולות להסתיים בתיקיית דואר הזבל של הנמען.</span><span class="sxs-lookup"><span data-stu-id="a9635-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="a9635-106">לקבלת מידע נוסף, ראה [מקורות מסירה יוצאים](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="a9635-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="a9635-107">כדי להימנע מתרחיש באמצעות מאגר הממסר, ודא שהודעות שהועברו/ממסר יפגשו באחד מהקריטריונים הבאים:</span><span class="sxs-lookup"><span data-stu-id="a9635-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="a9635-108">השולח היוצא הוא תחום מקובל של הדייר.</span><span class="sxs-lookup"><span data-stu-id="a9635-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="a9635-109">Sender Policy Framework (SPF) עובר כאשר ההודעה מגיעה Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a9635-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="a9635-110">DomainKeys Identified Mail (DKIM) בתחום שולח P2 עובר כאשר ההודעה מגיעה Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a9635-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="a9635-111">הודעות המנוהות לקריטריונים לעיל הבאות לא יעבירו דרך מאגר הממסרים.</span><span class="sxs-lookup"><span data-stu-id="a9635-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="a9635-112">אם רשומת ה- MX עבור התחום שלך מופנה לשרת של ספקים אחרים או לשרת מקומי, השתמש בסינון משופר כדי לוודא שאימות ה- SPF נכון עבור דואר אלקטרוני נכנס ולהימנע משליחה של דואר אלקטרוני דרך מאגר הממסרים.</span><span class="sxs-lookup"><span data-stu-id="a9635-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="a9635-113">**כיצד נוכל לדעת אם מאגר הממסר משפיע עלינו?**</span><span class="sxs-lookup"><span data-stu-id="a9635-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="a9635-114">אם הודעות הדואר האלקטרוני שהועברו או מועברות משתמשות באחד מהקריטריונים לעיל, הודעות לא ימסרו דרך מאגר הממסרים.</span><span class="sxs-lookup"><span data-stu-id="a9635-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="a9635-115">עם זאת, אם הודעה נשלחת דרך מאגר ממסר, ה- IP של השרת היוצא נמצא בטווח 40.95.0.0/16, שם השרת היוצא כולל **rly** בשם.</span><span class="sxs-lookup"><span data-stu-id="a9635-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

