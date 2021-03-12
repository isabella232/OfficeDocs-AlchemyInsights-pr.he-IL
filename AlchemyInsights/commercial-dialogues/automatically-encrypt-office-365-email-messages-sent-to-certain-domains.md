---
title: הצפנה אוטומטית של הודעות דואר אלקטרוני של Office 365 הנשלחות לתחומים מסוימים
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746051"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="adf2f-102">הצפנה אוטומטית של הודעות דואר אלקטרוני של Office 365 הנשלחות לתחומים מסוימים</span><span class="sxs-lookup"><span data-stu-id="adf2f-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="adf2f-103">מתוך [מרכז הניהול של Exchange](https://outlook.office365.com/ecp/), בחר באפשרות **זרימת דואר > כללים**.</span><span class="sxs-lookup"><span data-stu-id="adf2f-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="adf2f-104">לחץ על סמל **חדש (+)** ולאחר מכן לחץ על **החל את הצפנת ההודעות של Office 365 והגנה על זכויות על הודעות**.</span><span class="sxs-lookup"><span data-stu-id="adf2f-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="adf2f-105">תחת **שם**, הזן שם עבור הכלל, כגון *הצפנת הודעות הנשלחות אל contoso.com*.</span><span class="sxs-lookup"><span data-stu-id="adf2f-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="adf2f-106">תחת **החל כלל זה אם**, בחר **את התחום של הנמען >**.</span><span class="sxs-lookup"><span data-stu-id="adf2f-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="adf2f-107">הזן את שם התחום, כגון **contoso.com**.</span><span class="sxs-lookup"><span data-stu-id="adf2f-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="adf2f-108">לחץ על סמל **הוסף (+)** ולאחר מכן לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="adf2f-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="adf2f-109">לצד השדה **בצע את הפעולות הבאות** , לחץ על **בחר אחד**.</span><span class="sxs-lookup"><span data-stu-id="adf2f-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="adf2f-110">בתפריט הנפתח ' **תבנית RMS** ', בחר **באפשרות** **הצפן** ולאחר מכן לחץ על אישור.</span><span class="sxs-lookup"><span data-stu-id="adf2f-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="adf2f-111">(אם אינך רואה אפשרות זו, משמעות הדבר היא שהתוכנית שלך אינה כוללת הצפנה אוטומטית.</span><span class="sxs-lookup"><span data-stu-id="adf2f-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="adf2f-112">אך באפשרותך להוסיף אותה!)</span><span class="sxs-lookup"><span data-stu-id="adf2f-112">But you can add it!)</span></span>
9. <span data-ttu-id="adf2f-113">בחר באפשרות בחירה אופציונלית כלשהי (מתוך רשימה של בחירות אופציונליות שניתן לקבוע בשלב זה, שרבים מהן ניתנות לשמאל עם הגדרת ברירת המחדל עבור פשטות).</span><span class="sxs-lookup"><span data-stu-id="adf2f-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="adf2f-114">לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="adf2f-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="adf2f-115">תמיד תוכל לחזור ולערוך כלל זה מאוחר יותר.</span><span class="sxs-lookup"><span data-stu-id="adf2f-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="adf2f-116">לקבלת מידע נוסף אודות יצירת כללים עבור הצפנה, ראה [הגדרת כללי זרימת דואר כדי להצפין הודעות דואר אלקטרוני ב-Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="adf2f-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>