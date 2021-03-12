---
title: העברה אוטומטית של הודעות דואר אלקטרוני לתיבת הדואר של הארכיון
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
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746042"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="4c796-102">העברה אוטומטית של הודעות דואר אלקטרוני לתיבת הדואר של הארכיון</span><span class="sxs-lookup"><span data-stu-id="4c796-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="4c796-103">כך ניתן להגדיר מדיניות כדי להעביר באופן אוטומטי את הדואר האלקטרוני הישן של המשתמש לתיבת הדואר של הארכיון:</span><span class="sxs-lookup"><span data-stu-id="4c796-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="4c796-104">עבור אל [**ארכיון אבטחה & תאימות**](https://go.microsoft.com/fwlink/p/?linkid=2077143)  >  '**ממשל נתונים**  >   ' כדי לוודא שתיבת דואר של ארכיון הופעלה עבור המשתמש.</span><span class="sxs-lookup"><span data-stu-id="4c796-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="4c796-105">אם לא, לחץ על **הפוך לזמין** **בתיבת** האזהרה.</span><span class="sxs-lookup"><span data-stu-id="4c796-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="4c796-106">עבור אל [**מרכז הניהול של Exchange > ניהול תאימות > תגיות שמירה**](https://go.microsoft.com/fwlink/?linkid=2059104).</span><span class="sxs-lookup"><span data-stu-id="4c796-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="4c796-107">בחר את סמל + ולאחר מכן בחר **החל באופן אוטומטי על תיבת הדואר כולה**.</span><span class="sxs-lookup"><span data-stu-id="4c796-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="4c796-108">הקצה שם לתגית השמירה ובחר **העבר לארכיון**.</span><span class="sxs-lookup"><span data-stu-id="4c796-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="4c796-109">עבור תקופת השמירה, הזן את השעה הרצויה, כגון 90 ימים.</span><span class="sxs-lookup"><span data-stu-id="4c796-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="4c796-110">לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="4c796-110">Click **Save**.</span></span>
5. <span data-ttu-id="4c796-111">כעת צור מדיניות שמירה: בחר באפשרות מדיניות **שמירה**, בחר את הסמל כדי להוסיף מדיניות חדשה.</span><span class="sxs-lookup"><span data-stu-id="4c796-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="4c796-112">הקצה שם למדיניות השמירה ולאחר מכן לחץ וגלול כדי לחפש ולהוסיף את תג השמירה שיצרת זה עתה.</span><span class="sxs-lookup"><span data-stu-id="4c796-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="4c796-113">לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="4c796-113">Click **Save**.</span></span>
7. <span data-ttu-id="4c796-114">לבסוף, החל את מדיניות השמירה על תיבת הדואר של המשתמש: עדיין במרכז הניהול של Exchange, עבור אל  >  **תיבות הדואר** של הנמענים.</span><span class="sxs-lookup"><span data-stu-id="4c796-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="4c796-115">בחר את כל המשתמשים שברצונך להחיל עליהם את המדיניות ולאחר מכן בחר **Edit** (סמל העיפרון).</span><span class="sxs-lookup"><span data-stu-id="4c796-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="4c796-116">בתיבת הדו, לחץ על **תכונות תיבת דואר**.</span><span class="sxs-lookup"><span data-stu-id="4c796-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="4c796-117">תחת **מדיניות שמירה**, החל את המדיניות שיצרת זה עתה > **שמירה**.</span><span class="sxs-lookup"><span data-stu-id="4c796-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="4c796-118">לקבלת הוראות להחלת המדיניות על כל המשתמשים, ראה [החלת מדיניות שמירה על תיבות דואר](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span><span class="sxs-lookup"><span data-stu-id="4c796-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
