---
title: תיקון מדיניות חיבור
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746751"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="e3cdf-102">תיקון מדיניות חיבור</span><span class="sxs-lookup"><span data-stu-id="e3cdf-102">Fix connection policy</span></span>

<span data-ttu-id="e3cdf-103">הודעת הדואר האלקטרוני סומנה כבטוחה ונמסרה לתיבת הדואר הנכנס של המשתמש מאחר שכתובת ה-IP השולחת סומנה כבטוחה במדיניות מסנן החיבורים.</span><span class="sxs-lookup"><span data-stu-id="e3cdf-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="e3cdf-104">כדי לסקור את המדיניות, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="e3cdf-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="e3cdf-105">עבור אל [מרכז התאימות של & אבטחה של Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143)ולאחר מכן עבור אל מדיניות **ניהול האיום**  >    >  [נגד הודעות זבל](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="e3cdf-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="e3cdf-106">בכרטיסיה **התאמה אישית** , בחר את **מדיניות מסנן החיבורים** ולאחר מכן בחר **ערוך מדיניות**.</span><span class="sxs-lookup"><span data-stu-id="e3cdf-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="e3cdf-107">סקור את רשימת **ההיתרים של IP** .</span><span class="sxs-lookup"><span data-stu-id="e3cdf-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="e3cdf-108">ראה אם **הרשימה הבטוחה** מאופשרת.</span><span class="sxs-lookup"><span data-stu-id="e3cdf-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="e3cdf-109">Microsoft נרשמת כמנוי למקורות ספקים חיצוניים של שולחים מהימנים.</span><span class="sxs-lookup"><span data-stu-id="e3cdf-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="e3cdf-110">אם **הרשימה הבטוחה** מופעלת, שולחים מהימנים אלה לא מסומנים בטעות כדואר זבל.</span><span class="sxs-lookup"><span data-stu-id="e3cdf-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="e3cdf-111">אני ממליץ לבחור באפשרות זו, משום שהיא תקטין את מספר החיובים החיוביים הכוזבים (דואר טוב שמסווג כדואר זבל) שאתה מקבל.</span><span class="sxs-lookup"><span data-stu-id="e3cdf-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
