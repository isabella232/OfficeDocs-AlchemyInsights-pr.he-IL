---
title: חיפוש אירועים שבוצעו בכללי תיבת דואר נכנס
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429626"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="de083-102">חיפוש אירועים שבוצעו בכללי תיבת דואר נכנס</span><span class="sxs-lookup"><span data-stu-id="de083-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="de083-103">כאשר כללי תיבת דואר נכנס נוצרים, משתנים או נמחקים, האירועים נרשמים ביומן הביקורת.</span><span class="sxs-lookup"><span data-stu-id="de083-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="de083-104">כך ניתן לסקור אותם:</span><span class="sxs-lookup"><span data-stu-id="de083-104">Here's how to review them:</span></span>

1. <span data-ttu-id="de083-105">עבור אל [מרכז התאימות & אבטחה של Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="de083-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="de083-106">בחר חיפוש > חיפוש ביומן הביקורת.</span><span class="sxs-lookup"><span data-stu-id="de083-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="de083-107">אם אתה רואה הודעה שעליך להפעיל את הביקורת, הפעל אותה כעת.</span><span class="sxs-lookup"><span data-stu-id="de083-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="de083-108">אם תכונה זו אינה מופעלת, תוצאות החיפוש לא יוכלו למשוך נתונים מתאריכים קודמים.</span><span class="sxs-lookup"><span data-stu-id="de083-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="de083-109">בחר את השדה פעילויות ואתר את פעילויות תיבת הדואר של Exchange ולאחר מכן בחר New-InboxRule יצירת כלל תיבת דואר נכנס מ-Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="de083-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="de083-110">לאחר שתסיים, לחץ מחוץ לחלונית כדי למזער את החלונית פעילויות.</span><span class="sxs-lookup"><span data-stu-id="de083-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="de083-111">ציין את טווח התאריכים ולאחר מכן, בשדה משתמשים, בחר את שם המשתמש עבור המשתמש שברצונך לחקור.</span><span class="sxs-lookup"><span data-stu-id="de083-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="de083-112">באפשרותך לבחור יותר ממשתמש אחד בכל פעם.</span><span class="sxs-lookup"><span data-stu-id="de083-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="de083-113">בחר חיפוש.</span><span class="sxs-lookup"><span data-stu-id="de083-113">Select Search.</span></span> <span data-ttu-id="de083-114">הפעילויות מופיעות תחת תוצאות.</span><span class="sxs-lookup"><span data-stu-id="de083-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="de083-115">כדי להציג פרטים, בחר פעילות ולאחר מכן בחר מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="de083-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="de083-116">תחת המקטע פרמטרים, באפשרותך לראות את שם הכלל, ערכת התנאים והפעולות שבהן הכלל יתבצע.</span><span class="sxs-lookup"><span data-stu-id="de083-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="de083-117">לקבלת מידע נוסף, ראה חיפוש ביומן הביקורת של Office 365 כדי לפתור תרחישים נפוצים.</span><span class="sxs-lookup"><span data-stu-id="de083-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>