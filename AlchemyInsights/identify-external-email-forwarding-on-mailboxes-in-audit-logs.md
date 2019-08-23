---
title: לזהות העברת דואר אלקטרוני חיצוני על תיבות דואר ביומני ביקורת
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7defd0902e8c8bebae9c7bfee72c3199cbc1909f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539102"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="442b1-102">לזהות בעת העברת דואר אלקטרוני חיצוני נקבעה עבור תיבות דואר</span><span class="sxs-lookup"><span data-stu-id="442b1-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="442b1-103">כאשר משתמש Office 365 קובע תצורה של העברת דואר אלקטרוני חיצוני דואר, הפעילות תתבצע ביקורת כחלק cmdlet **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="442b1-103">When an Office 365  user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="442b1-104">באפשרותך לראות את הפעילות באמצעות חיפוש יומן ביקורת ב- & אבטחה מרכז תאימות.</span><span class="sxs-lookup"><span data-stu-id="442b1-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="442b1-105">היכנס אל [מרכז התאימות של Office 365 אבטחה &](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="442b1-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="442b1-106">עבור אל **חיפוש** > דף**החיפוש יומן הביקורת** .</span><span class="sxs-lookup"><span data-stu-id="442b1-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="442b1-107">בחר את טווח התאריכים בשדות **תאריך התחלה** ותאריך **סיום** .</span><span class="sxs-lookup"><span data-stu-id="442b1-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="442b1-108">אין צורך לציין שם משתמש.</span><span class="sxs-lookup"><span data-stu-id="442b1-108">You don't need to specify a username.</span></span> <span data-ttu-id="442b1-109">ודא שהשדה **פעילויות** מוגדר להצגת **תוצאות עבור כל הפעילויות**.</span><span class="sxs-lookup"><span data-stu-id="442b1-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="442b1-110">לחץ על **חיפוש**.</span><span class="sxs-lookup"><span data-stu-id="442b1-110">Click **Search**.</span></span>

<span data-ttu-id="442b1-111">בתוצאות, לחץ על **סינון תוצאות** והקלד **Set-Mailbox** בתיבה מסנן פעילות.</span><span class="sxs-lookup"><span data-stu-id="442b1-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="442b1-112">בחר את רשומת הביקורת בתוצאות.</span><span class="sxs-lookup"><span data-stu-id="442b1-112">Select an audit record in the results.</span></span> <span data-ttu-id="442b1-113">תפריט נשלף של **פרטים** , לחץ על **מידע נוסף**.</span><span class="sxs-lookup"><span data-stu-id="442b1-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="442b1-114">יש לך להסתכל על הפרטים של כל רשומת הביקורת כדי לקבוע אם הפעילות קשורה דוא ל העברה.</span><span class="sxs-lookup"><span data-stu-id="442b1-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="442b1-115">**ObjectId**: הערך הכינוי של תיבת הדואר שהשתנה.</span><span class="sxs-lookup"><span data-stu-id="442b1-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="442b1-116">**פרמטרים**: _ForwardingSmtpAddress_ מציין את כתובת הדואר האלקטרוני של היעד.</span><span class="sxs-lookup"><span data-stu-id="442b1-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="442b1-117">**מזהה משתמש**: המשתמש שתצורתו נקבעה העברת דואר אלקטרוני בתיבת הדואר בשדה **ObjectId** .</span><span class="sxs-lookup"><span data-stu-id="442b1-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="442b1-118">לקבלת מידע נוסף, ראה [קביעת שהגדיר העברה עבור תיבת דואר אלקטרוני](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="442b1-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
