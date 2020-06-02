---
title: זיהוי העברת דואר אלקטרוני חיצוני בתיבות דואר ביומני ביקורת
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 592eb92e4b0fe0f9da2fa20bb93ffa4fbbb76662
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508953"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="67783-102">זיהוי כאשר תצורת העברת דואר אלקטרוני חיצונית מוגדרת בתיבות דואר</span><span class="sxs-lookup"><span data-stu-id="67783-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="67783-103">כאשר משתמש של Microsoft 365 מגדיר העברה של דואר אלקטרוני חיצוני בתיבת דואר, הפעילות מתבצעת ביקורת כחלק מיישומון ה **-Cmdlet Set-mailbox** .</span><span class="sxs-lookup"><span data-stu-id="67783-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="67783-104">באפשרותך לראות את הפעילות באמצעות חיפוש יומן ביקורת במרכז התאימות של אבטחה _ אמפר _.</span><span class="sxs-lookup"><span data-stu-id="67783-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="67783-105">היכנס ל- [Microsoft 365 האבטחה _ אמפר _ מרכז התאימות](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="67783-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="67783-106">עבור אל דף **Search**  >  **החיפוש של יומן ביקורת** החיפוש.</span><span class="sxs-lookup"><span data-stu-id="67783-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="67783-107">בחר את טווח התאריכים **בתאריך ההתחלה** ושדות **הסיום** .</span><span class="sxs-lookup"><span data-stu-id="67783-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="67783-108">אין צורך לציין שם משתמש.</span><span class="sxs-lookup"><span data-stu-id="67783-108">You don't need to specify a username.</span></span> <span data-ttu-id="67783-109">ודא שהשדה **פעילויות** מוגדר **להצגת תוצאות עבור כל הפעילויות**.</span><span class="sxs-lookup"><span data-stu-id="67783-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="67783-110">לחץ על **חיפוש**.</span><span class="sxs-lookup"><span data-stu-id="67783-110">Click **Search**.</span></span>

<span data-ttu-id="67783-111">בתוצאות, לחץ על **סנן תוצאות** וסוג **ערכת תיבות דואר** בתיבה מסנן פעילות.</span><span class="sxs-lookup"><span data-stu-id="67783-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="67783-112">בחר רשומת ביקורת בתוצאות.</span><span class="sxs-lookup"><span data-stu-id="67783-112">Select an audit record in the results.</span></span> <span data-ttu-id="67783-113">בתפריט **הפרטי** , לחץ על **מידע נוסף**.</span><span class="sxs-lookup"><span data-stu-id="67783-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="67783-114">עליך לבדוק את הפרטים של כל רשומת ביקורת כדי לקבוע אם הפעילות קשורה להעברת דואר אלקטרוני.</span><span class="sxs-lookup"><span data-stu-id="67783-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="67783-115">**אובייtid**: ערך הכינוי של תיבת הדואר שהשתנתה.</span><span class="sxs-lookup"><span data-stu-id="67783-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="67783-116">**פרמטרים**: _כתובת השולח_ מציינת את כתובת האימייל של היעד.</span><span class="sxs-lookup"><span data-stu-id="67783-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="67783-117">**Userid**: המשתמש שהגדיר העברת דואר אלקטרוני בתיבת הדואר בשדה **אובייtid** .</span><span class="sxs-lookup"><span data-stu-id="67783-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="67783-118">לקבלת מידע נוסף, ראה [קביעה מי הגדיר העברת דואר אלקטרוני עבור תיבת דואר](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="67783-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
