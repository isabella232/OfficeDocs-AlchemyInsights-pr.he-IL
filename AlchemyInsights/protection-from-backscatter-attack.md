---
title: הגנה מפני התקפה של Backscatter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036072"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="55cbc-102">הגנה מפני התקפה של Backscatter</span><span class="sxs-lookup"><span data-stu-id="55cbc-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="55cbc-103">Backscatter הוא דוחות אי-מסירה (המכונים גם ' הודעות ' Ndr ' או ' הקפץ ') שאתה מקבל עבור הודעות שלא שלחת.</span><span class="sxs-lookup"><span data-stu-id="55cbc-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="55cbc-104">שולחי הודעות זבל מזייפים (מזייפים) את הכתובת **מאת:** ההודעות שלהם, ולעתים קרובות הם משתמשים בכתובות דואר אלקטרוני אמיתיות כדי להעניק אמינות להודעות שלהם.</span><span class="sxs-lookup"><span data-stu-id="55cbc-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="55cbc-105">כך, כאשר שולחי הודעות זבל שולחים הודעות לנמענים שאינם קיימים, שרת הדואר האלקטרוני של היעד מרומה למעשה להחזרת ההודעה שאינה ניתנת למסירה בהודעת NDR לשולח המזייף בכתובת **From:** .</span><span class="sxs-lookup"><span data-stu-id="55cbc-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="55cbc-106">מידע נוסף ניתן למצוא ב- [Backscatter ב-EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span><span class="sxs-lookup"><span data-stu-id="55cbc-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="55cbc-107">**הפעלת הגנה מפני Backscatter**</span><span class="sxs-lookup"><span data-stu-id="55cbc-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="55cbc-108">כדי להפוך הגנה של Backscatter לזמינה, בצע את הנתיב שלהלן.</span><span class="sxs-lookup"><span data-stu-id="55cbc-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="55cbc-109">**protection.office.com > מדיניות ניהול האיום > > ספאם > בחירת מדיניות מסנן דואר הזבל ועריכת מדיניות > מאפייני דואר זבל > סימון כהודעת זבל > NDR backscatter > הגדר אותה "On"**</span><span class="sxs-lookup"><span data-stu-id="55cbc-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="55cbc-110">אם אתה סבור שהחשבון נחשף, עיין בפרטים הבאים:</span><span class="sxs-lookup"><span data-stu-id="55cbc-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="55cbc-111">תגובה לחשבון דואר אלקטרוני שנחשף</span><span class="sxs-lookup"><span data-stu-id="55cbc-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="55cbc-112">הסרת משתמשים חסומים מפורטל המשתמשים המוגבלים ב-Office 365</span><span class="sxs-lookup"><span data-stu-id="55cbc-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



