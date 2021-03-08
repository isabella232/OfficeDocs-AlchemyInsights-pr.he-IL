---
title: הצפנה אוטומטית של הודעות דואר אלקטרוני מסוימות של Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524899"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="f0f18-102">הצפנה אוטומטית של הודעות דואר אלקטרוני מסוימות של Office 365</span><span class="sxs-lookup"><span data-stu-id="f0f18-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="f0f18-103">באפשרותך להצפין באופן אוטומטי הודעות שמשתמשים שולחים לאנשים חיצוניים או לארגונים מסוימים.</span><span class="sxs-lookup"><span data-stu-id="f0f18-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="f0f18-104">לשם כך, בצע את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="f0f18-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="f0f18-105">מתוך [מרכז הניהול של Exchange](https://outlook.office365.com/ecp/), בחר באפשרות **זרימת דואר > כללים**.</span><span class="sxs-lookup"><span data-stu-id="f0f18-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="f0f18-106">לחץ על סמל **חדש (+)** ולאחר מכן לחץ על **החל את הצפנת ההודעות של Office 365 והגנה על זכויות על הודעות**.</span><span class="sxs-lookup"><span data-stu-id="f0f18-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="f0f18-107">תחת **שם**, הזן שם עבור הכלל, כגון *הצפנת הודעות הנשלחות אל DrToniRamos@gmail.com*.</span><span class="sxs-lookup"><span data-stu-id="f0f18-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="f0f18-108">תחת **החל כלל זה אם**, בחר **את ה> נמען הוא אדם זה**.</span><span class="sxs-lookup"><span data-stu-id="f0f18-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="f0f18-109">בחלון **' בחירת חברים** ', בחר את שם האדם שברצונך להחיל עליו את כלל ההצפנה ולאחר מכן לחץ על **הוסף**.</span><span class="sxs-lookup"><span data-stu-id="f0f18-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="f0f18-110">לאחר שתסיים להוסיף משתמשים, לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="f0f18-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="f0f18-111">לצד השדה **בצע את הפעולות הבאות** , לחץ על **בחר אחד**.</span><span class="sxs-lookup"><span data-stu-id="f0f18-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="f0f18-112">בתפריט הנפתח ' **תבנית RMS** ', בחר **באפשרות** **הצפן** ולאחר מכן לחץ על אישור.</span><span class="sxs-lookup"><span data-stu-id="f0f18-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="f0f18-113">(אם אינך רואה אפשרות זו, משמעות הדבר היא שהתוכנית שלך אינה כוללת הצפנה אוטומטית.</span><span class="sxs-lookup"><span data-stu-id="f0f18-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="f0f18-114">אך באפשרותך להוסיף אותה!)</span><span class="sxs-lookup"><span data-stu-id="f0f18-114">But you can add it!)</span></span>
9. <span data-ttu-id="f0f18-115">בחר באפשרות בחירה אופציונלית כלשהי (מתוך רשימה של בחירות אופציונליות שניתן לקבוע בשלב זה, שרבים מהן ניתנות לשמאל עם הגדרת ברירת המחדל עבור פשטות).</span><span class="sxs-lookup"><span data-stu-id="f0f18-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="f0f18-116">לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="f0f18-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="f0f18-117">תמיד תוכל לחזור ולערוך כלל זה מאוחר יותר.</span><span class="sxs-lookup"><span data-stu-id="f0f18-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="f0f18-118">לקבלת מידע נוסף אודות יצירת כללים עבור הצפנה, ראה [הגדרת כללי זרימת דואר כדי להצפין הודעות דואר אלקטרוני ב-Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="f0f18-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

