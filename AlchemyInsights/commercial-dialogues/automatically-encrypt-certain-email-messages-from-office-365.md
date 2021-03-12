---
title: הצפנה אוטומטית של הודעות דואר אלקטרוני מסוימות מ-office 365
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
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746135"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="09e83-102">הצפנה אוטומטית של הודעות דואר אלקטרוני מסוימות מ-office 365</span><span class="sxs-lookup"><span data-stu-id="09e83-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="09e83-103">מתוך [מרכז הניהול של Exchange](https://outlook.office365.com/ecp/), בחר באפשרות **זרימת דואר > כללים**.</span><span class="sxs-lookup"><span data-stu-id="09e83-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="09e83-104">לחץ על סמל **חדש (+)** ולאחר מכן לחץ על **החל את הצפנת ההודעות של Office 365 והגנה על זכויות על הודעות**.</span><span class="sxs-lookup"><span data-stu-id="09e83-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="09e83-105">תחת **שם**, הזן שם עבור הכלל, כגון *הצפן את כל ההודעות*.</span><span class="sxs-lookup"><span data-stu-id="09e83-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="09e83-106">תחת **החל כלל זה אם**, בחר **[החל על כל ההודעות]**.</span><span class="sxs-lookup"><span data-stu-id="09e83-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="09e83-107">לצד השדה **בצע את הפעולות הבאות** , לחץ על **בחר אחד**.</span><span class="sxs-lookup"><span data-stu-id="09e83-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="09e83-108">בתפריט הנפתח ' **תבנית RMS** ', בחר **באפשרות** **הצפן** ולאחר מכן לחץ על אישור.</span><span class="sxs-lookup"><span data-stu-id="09e83-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="09e83-109">(אם אינך רואה אפשרות זו, משמעות הדבר היא שהתוכנית שלך אינה כוללת הצפנה אוטומטית.</span><span class="sxs-lookup"><span data-stu-id="09e83-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="09e83-110">אך באפשרותך להוסיף אותה!)</span><span class="sxs-lookup"><span data-stu-id="09e83-110">But you can add it!)</span></span>
7. <span data-ttu-id="09e83-111">סמן את תיבת הסימון בדוק **כלל זה עם רמת חומרה** ולאחר מכן בחר את הרמה הרצויה.</span><span class="sxs-lookup"><span data-stu-id="09e83-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="09e83-112">אם לחברה שלך יש התחייבויות חוזיות כדי לשלוח את כל הודעות הדואר האלקטרוני מוצפנות, אני ממליץ להגדיר את הרמה **לגבוהה**.</span><span class="sxs-lookup"><span data-stu-id="09e83-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="09e83-113">תחת **בחר מודל עבור כלל זה**, לחץ על **אכוף**.</span><span class="sxs-lookup"><span data-stu-id="09e83-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="09e83-114">בחר באפשרות בחירה אופציונלית כלשהי (מתוך רשימה של בחירות אופציונליות שניתן לקבוע בשלב זה, שרבים מהן ניתנות לשמאל עם הגדרת ברירת המחדל עבור פשטות).</span><span class="sxs-lookup"><span data-stu-id="09e83-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="09e83-115">לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="09e83-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="09e83-116">תמיד תוכל לחזור ולערוך כלל זה מאוחר יותר.</span><span class="sxs-lookup"><span data-stu-id="09e83-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="09e83-117">לקבלת מידע נוסף אודות יצירת כללים עבור הצפנה, ראה [הגדרת כללי זרימת דואר כדי להצפין הודעות דואר אלקטרוני ב-Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="09e83-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

