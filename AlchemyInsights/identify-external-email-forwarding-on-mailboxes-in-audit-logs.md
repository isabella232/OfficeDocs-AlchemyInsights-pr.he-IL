---
title: זיהוי העברת דואר אלקטרוני חיצונית בתיבות דואר ביומני ביקורת
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696298"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="89eeb-102">זיהוי כאשר העברת דואר אלקטרוני חיצונית מוגדרת בתיבות דואר</span><span class="sxs-lookup"><span data-stu-id="89eeb-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="89eeb-103">כאשר משתמש של Microsoft 365 קובע את התצורה של העברת דואר אלקטרוני חיצוני בתיבת דואר, הפעילות מתבצעת ביקורת כחלק מ **-Cmdlet Set-mailbox** .</span><span class="sxs-lookup"><span data-stu-id="89eeb-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="89eeb-104">באפשרותך לראות את הפעילות באמצעות חיפוש ביומן הביקורת במרכז התאימות של אבטחה &.</span><span class="sxs-lookup"><span data-stu-id="89eeb-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="89eeb-105">היכנס [למרכז התאימות של Microsoft 365 Security &](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="89eeb-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="89eeb-106">עבור אל דף **Search**  >  **החיפוש ביומן ביקורת** חיפוש.</span><span class="sxs-lookup"><span data-stu-id="89eeb-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="89eeb-107">בחר את טווח התאריכים בשדות **תאריך התחלה** **ותאריך סיום** .</span><span class="sxs-lookup"><span data-stu-id="89eeb-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="89eeb-108">אין צורך לציין שם משתמש.</span><span class="sxs-lookup"><span data-stu-id="89eeb-108">You don't need to specify a username.</span></span> <span data-ttu-id="89eeb-109">אימות השדה ' **פעילויות** ' מוגדר **לתצוגת תוצאות עבור כל הפעילויות**.</span><span class="sxs-lookup"><span data-stu-id="89eeb-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="89eeb-110">לחץ על **חיפוש**.</span><span class="sxs-lookup"><span data-stu-id="89eeb-110">Click **Search**.</span></span>

<span data-ttu-id="89eeb-111">בתוצאות, לחץ על **סנן תוצאות** והקלד **ערכת תיבת דואר** בתיבה מסנן פעילות.</span><span class="sxs-lookup"><span data-stu-id="89eeb-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="89eeb-112">בחר רשומת ביקורת בתוצאות.</span><span class="sxs-lookup"><span data-stu-id="89eeb-112">Select an audit record in the results.</span></span> <span data-ttu-id="89eeb-113">בנשלף של **הפרטים** , לחץ על **מידע נוסף**.</span><span class="sxs-lookup"><span data-stu-id="89eeb-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="89eeb-114">עליך לעיין בפרטים של כל רשומת ביקורת כדי לקבוע אם הפעילות קשורה להעברת דואר אלקטרוני.</span><span class="sxs-lookup"><span data-stu-id="89eeb-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="89eeb-115">**ObjectId**: ערך הכינוי של תיבת הדואר שהשתנתה.</span><span class="sxs-lookup"><span data-stu-id="89eeb-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="89eeb-116">**פרמטרים**: _ForwardingSmtpAddress_ מציין את כתובת הדואר האלקטרוני המהווה יעד.</span><span class="sxs-lookup"><span data-stu-id="89eeb-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="89eeb-117">**מזהה**משתמש: המשתמש שהגדיר את העברת הדואר האלקטרוני בתיבת הדואר בשדה **ObjectId** .</span><span class="sxs-lookup"><span data-stu-id="89eeb-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="89eeb-118">לקבלת מידע נוסף, ראה [קביעה מי הגדיר העברת דואר אלקטרוני עבור תיבת דואר](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="89eeb-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
