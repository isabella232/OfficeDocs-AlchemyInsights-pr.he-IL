---
title: קריאת יומני ביקורת עבור אירועים שנמחקו
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482261"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="e74fe-102">קריאת יומני ביקורת עבור אירועים שנמחקו</span><span class="sxs-lookup"><span data-stu-id="e74fe-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="e74fe-103">כך ניתן לעשות זאת:</span><span class="sxs-lookup"><span data-stu-id="e74fe-103">Here's how to do this:</span></span>

1. <span data-ttu-id="e74fe-104">עבור אל [מרכז התאימות & אבטחה של Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="e74fe-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="e74fe-105">בחר חיפוש  >  [**ביומן הביקורת**](https://go.microsoft.com/fwlink/?linkid=2103759)של חיפוש.</span><span class="sxs-lookup"><span data-stu-id="e74fe-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="e74fe-106">אם אתה רואה הודעה שעליך להפעיל את התכונה, קדימה והפעל אותה כעת.</span><span class="sxs-lookup"><span data-stu-id="e74fe-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="e74fe-107">אם התכונה אינה מופעלת, תוצאות החיפוש לא יוכלו למשוך נתונים מתאריכים קודמים.</span><span class="sxs-lookup"><span data-stu-id="e74fe-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="e74fe-108">בחר **פעילויות** ולאחר מכן אתר את **פעילויות תיבת הדואר של Exchange**.</span><span class="sxs-lookup"><span data-stu-id="e74fe-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="e74fe-109">בחר את **ההודעות שנמחקו מהתיקיה ' פריטים שנמחקו** ' **והעברת הודעות לאפשרויות התיקיה ' פריטים שנמחקו** '.</span><span class="sxs-lookup"><span data-stu-id="e74fe-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="e74fe-110">לאחר שתסיים, לחץ מחוץ לחלונית כדי למזער את החלונית **פעילויות** .</span><span class="sxs-lookup"><span data-stu-id="e74fe-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="e74fe-111">ציין את טווח התאריכים ולאחר מכן, בתיבה **משתמשים** , בחר את שם המשתמש עבור המשתמש שברצונך לחקור.</span><span class="sxs-lookup"><span data-stu-id="e74fe-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="e74fe-112">באפשרותך לבחור יותר ממשתמש אחד בכל פעם.</span><span class="sxs-lookup"><span data-stu-id="e74fe-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="e74fe-113">בחר **חיפוש**.</span><span class="sxs-lookup"><span data-stu-id="e74fe-113">Select **Search**.</span></span> <span data-ttu-id="e74fe-114">הפעילויות מופיעות תחת **תוצאות**.</span><span class="sxs-lookup"><span data-stu-id="e74fe-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="e74fe-115">כדי להציג את הפרטים, בחר פעילות ולאחר מכן בחר **מידע נוסף**.</span><span class="sxs-lookup"><span data-stu-id="e74fe-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="e74fe-116">מידע נוסף אודות הפריט שנמחק, כגון שורת הנושא ומיקום הפריט בעת המחיקה, מוצג בשדה **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="e74fe-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="e74fe-117">לא ניתן לשחזר פריטים שנמחקו באמצעות התכונה ' יומן ביקורת '.</span><span class="sxs-lookup"><span data-stu-id="e74fe-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="e74fe-118">כדי לשחזר פריטים שנמחקו, ראה [שחזור פריטים שנמחקו או דואר אלקטרוני ב-Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span><span class="sxs-lookup"><span data-stu-id="e74fe-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="e74fe-119">לקבלת מידע נוסף, ראה [חיפוש ביומן הביקורת של Office 365 כדי לפתור תרחישים נפוצים](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="e74fe-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
