---
title: גלה מי הגדיר העברה בתיבת דואר וכיצד
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429614"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="93b3c-102">גלה מי הגדיר העברה בתיבת דואר וכיצד</span><span class="sxs-lookup"><span data-stu-id="93b3c-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="93b3c-103">אם הוגדרה העברה חיצונית בתיבת דואר, הפעילות מתבצעת ביקורת כחלק מ-cmdlet הSet-Mailbox.</span><span class="sxs-lookup"><span data-stu-id="93b3c-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="93b3c-104">כך תוכל למצוא את הפעילות ביומן הביקורת:</span><span class="sxs-lookup"><span data-stu-id="93b3c-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="93b3c-105">עבור אל [מרכז התאימות & אבטחה של Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="93b3c-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="93b3c-106">בחר חיפוש >  **ביומן הביקורת** של חיפוש.</span><span class="sxs-lookup"><span data-stu-id="93b3c-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="93b3c-107">אם אתה רואה הודעה שעליך להפעיל את הביקורת, הפעל אותה כעת.</span><span class="sxs-lookup"><span data-stu-id="93b3c-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="93b3c-108">אם תכונה זו אינה מופעלת, תוצאות החיפוש לא יוכלו למשוך נתונים מתאריכים קודמים.</span><span class="sxs-lookup"><span data-stu-id="93b3c-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="93b3c-109">ודא שהשדה **פעילויות** מוגדר **להציג תוצאות עבור כל הפעילויות** (ברירת המחדל).</span><span class="sxs-lookup"><span data-stu-id="93b3c-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="93b3c-110">ציין את טווח התאריכים.</span><span class="sxs-lookup"><span data-stu-id="93b3c-110">Specify the date range.</span></span> <span data-ttu-id="93b3c-111">אין צורך לציין שם משתמש.</span><span class="sxs-lookup"><span data-stu-id="93b3c-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="93b3c-112">בחר **חיפוש**.</span><span class="sxs-lookup"><span data-stu-id="93b3c-112">Select **Search**.</span></span> <span data-ttu-id="93b3c-113">הפעילויות מופיעות תחת **תוצאות**.</span><span class="sxs-lookup"><span data-stu-id="93b3c-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="93b3c-114">בחר באפשרות **מסנן תוצאות** ולאחר מכן הזן **Set-mailbox** בשדה מסנן **פעילות** .</span><span class="sxs-lookup"><span data-stu-id="93b3c-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="93b3c-115">פעולה זו מחזירה את כל פעילויות **הערכה-תיבת דואר** .</span><span class="sxs-lookup"><span data-stu-id="93b3c-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="93b3c-116">כדי להציג את הפרטים, בחר פעילות ולאחר מכן בחר **מידע נוסף**.</span><span class="sxs-lookup"><span data-stu-id="93b3c-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="93b3c-117">תחת **פרמטרים** באפשרותך לראות את כתובת הדואר האלקטרוני להעברה שהוגדרה בתיבת הדואר.</span><span class="sxs-lookup"><span data-stu-id="93b3c-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="93b3c-118">**מזהה** המשתמש מייצג את המשתמש שהגדיר העברה חיצונית בתיבת הדואר.</span><span class="sxs-lookup"><span data-stu-id="93b3c-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="93b3c-119">לקבלת מידע נוסף, ראה [חיפוש ביומן הביקורת של Office 365 כדי לפתור תרחישים נפוצים](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="93b3c-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>