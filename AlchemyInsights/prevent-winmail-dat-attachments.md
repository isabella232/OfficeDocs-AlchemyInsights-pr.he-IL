---
title: 2589 עזור למנוע קבצים מצורפים של Winmail. dat בהודעות דואר אלקטרוני מהארגון שלך
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2589
ms.assetid: ''
ms.openlocfilehash: f67c4146af419a590651c8e0673fd59fabd7eae7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47693736"
---
# <a name="help-prevent-winmaildat-attachments-in-email-messages-from-your-organization"></a><span data-ttu-id="333ed-102">סיוע במניעת קבצים מצורפים של Winmail. dat בהודעות דואר אלקטרוני מהארגון שלך</span><span class="sxs-lookup"><span data-stu-id="333ed-102">Help prevent Winmail.dat attachments in email messages from your organization</span></span>

<span data-ttu-id="333ed-103">כמנהל מערכת, נסה את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="333ed-103">As an admin, try these steps:</span></span>

1. <span data-ttu-id="333ed-104">פתח את [מרכז הניהול של Exchange](https://outlook.office365.com/ecp/).</span><span class="sxs-lookup"><span data-stu-id="333ed-104">Open the [Exchange admin center](https://outlook.office365.com/ecp/).</span></span>

2. <span data-ttu-id="333ed-105">עבור אל **Mail flow**  >  **תחומים מרוחקים**של זרימת דואר.</span><span class="sxs-lookup"><span data-stu-id="333ed-105">Go to **Mail flow** > **Remote domains**.</span></span>

3. <span data-ttu-id="333ed-106">בחר את התחום המרוחק המהווה ברירת מחדל בשם **ברירת המחדל**ולאחר מכן לחץ על **ערוך**.</span><span class="sxs-lookup"><span data-stu-id="333ed-106">Select the default remote domain named **Default**, and then click **Edit**.</span></span>

4. <span data-ttu-id="333ed-107">במקטע **השתמש בתבנית טקסט עשיר** , בחר **לעולם לא**.</span><span class="sxs-lookup"><span data-stu-id="333ed-107">In the **Use Rich-text format** section, select **Never**.</span></span>

<span data-ttu-id="333ed-108">לקבלת מידע נוסף, ראה [ציון תבנית ההודעה עבור תחומים מרוחקים](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format).</span><span class="sxs-lookup"><span data-stu-id="333ed-108">For more information, see [Specify the message format for remote domains](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format).</span></span>
