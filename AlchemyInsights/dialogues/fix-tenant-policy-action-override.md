---
title: תיקון מדיניות דייר (עקיפת פעולה)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694063"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="26b60-102">תיקון מדיניות דייר (עקיפת פעולה)</span><span class="sxs-lookup"><span data-stu-id="26b60-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="26b60-103">מדיניות למניעת הודעות זבל בדייר שלך השפיעה על הודעה זו.</span><span class="sxs-lookup"><span data-stu-id="26b60-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="26b60-104">כדי לסקור את המדיניות, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="26b60-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="26b60-105">עבור אל [מרכז התאימות של & אבטחה של Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143)ולאחר מכן עבור אל מדיניות **ניהול האיום**  >    >  [נגד הודעות זבל](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="26b60-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="26b60-106">בדוק אם **מקור מדיניות** מציין את הפרטים הבאים:  **Add-Xheader/ModifySubject/ניתוב מחדש/מחיקה/אין הודעת פעולה/עותק מוסתר**</span><span class="sxs-lookup"><span data-stu-id="26b60-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="26b60-107">אם כן, בכרטיסיה **התאמה אישית** , סמן את הגדרות המדיניות שהשפיעו על ההודעה.</span><span class="sxs-lookup"><span data-stu-id="26b60-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="26b60-108">ייתכן **שההגדרות הרגילות** שהוחלו על כל לקוחות Exchange Online השפיעו על ההודעה.</span><span class="sxs-lookup"><span data-stu-id="26b60-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="26b60-109">לקבלת מידע נוסף אודות קביעת התצורה של פריטי מדיניות של מסנן דואר זבל, ראה [קביעת תצורה של מדיניות מסנן דואר הזבל](https://go.microsoft.com/fwlink/?linkid=2101431)</span><span class="sxs-lookup"><span data-stu-id="26b60-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
