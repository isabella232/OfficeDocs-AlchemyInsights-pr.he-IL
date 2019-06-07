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
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 518e4dd485ee7c54ce83e65794152e32f4c3a836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752002"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="62fd4-102">לזהות בעת העברת דואר אלקטרוני חיצוני נקבעה עבור תיבות דואר</span><span class="sxs-lookup"><span data-stu-id="62fd4-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="62fd4-103">כאשר משתמש מגדיר את העברת דואר אלקטרוני חיצוני דואר, הפעילות תתבצע ביקורת כחלק cmdlet **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="62fd4-103">When a user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="62fd4-104">באפשרותך לראות את הפעילות באמצעות חיפוש יומן ביקורת ב- & אבטחה מרכז תאימות.</span><span class="sxs-lookup"><span data-stu-id="62fd4-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="62fd4-105">היכנס אל [מרכז התאימות של Office 365 אבטחה &](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="62fd4-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="62fd4-106">לחץ על **חיפוש ויצירת החקירה** ובחר באפשרות **החיפוש יומן ביקורת**.</span><span class="sxs-lookup"><span data-stu-id="62fd4-106">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="62fd4-107">בחר את טווח התאריכים בשדות **תאריך התחלה** ותאריך **סיום** .</span><span class="sxs-lookup"><span data-stu-id="62fd4-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="62fd4-108">אין צורך לציין שם משתמש.</span><span class="sxs-lookup"><span data-stu-id="62fd4-108">You don't need to specify a username.</span></span> <span data-ttu-id="62fd4-109">ודא שהשדה **פעילויות** מוגדר להצגת **תוצאות עבור כל הפעילויות**.</span><span class="sxs-lookup"><span data-stu-id="62fd4-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="62fd4-110">לחץ על **חיפוש**.</span><span class="sxs-lookup"><span data-stu-id="62fd4-110">Click **Search**.</span></span>

<span data-ttu-id="62fd4-111">בתוצאות, לחץ על **סינון תוצאות** והקלד **Set-Mailbox** בתיבה מסנן פעילות.</span><span class="sxs-lookup"><span data-stu-id="62fd4-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="62fd4-112">בחר את רשומת הביקורת בתוצאות.</span><span class="sxs-lookup"><span data-stu-id="62fd4-112">Select an audit record in the results.</span></span> <span data-ttu-id="62fd4-113">תפריט נשלף של **פרטים** , לחץ על **מידע נוסף**.</span><span class="sxs-lookup"><span data-stu-id="62fd4-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="62fd4-114">יש לך להסתכל על הפרטים של כל רשומת הביקורת כדי לקבוע אם הפעילות קשורה דוא ל העברה.</span><span class="sxs-lookup"><span data-stu-id="62fd4-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="62fd4-115">**ObjectId**: הערך הכינוי של תיבת הדואר שהשתנה.</span><span class="sxs-lookup"><span data-stu-id="62fd4-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="62fd4-116">**פרמטרים**: _ForwardingSmtpAddress_ מציין את כתובת הדואר האלקטרוני של היעד.</span><span class="sxs-lookup"><span data-stu-id="62fd4-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="62fd4-117">**מזהה משתמש**: המשתמש שתצורתו נקבעה העברת דואר אלקטרוני בתיבת הדואר בשדה **ObjectId** .</span><span class="sxs-lookup"><span data-stu-id="62fd4-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="62fd4-118">לקבלת מידע נוסף, ראה [קביעת שהגדיר העברה עבור תיבת דואר אלקטרוני](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="62fd4-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
