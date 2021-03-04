---
title: איתור כתובת ה-IP ביומן הביקורת
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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429506"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="ebb10-102">איתור כתובת ה-IP ביומן הביקורת</span><span class="sxs-lookup"><span data-stu-id="ebb10-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="ebb10-103">כתובת ה-IP התואמת לפעילות שבוצעה על-ידי משתמש או מנהל מערכת מוצגת ביומני הביקורת.</span><span class="sxs-lookup"><span data-stu-id="ebb10-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="ebb10-104">פרטי הלקוח נרשמים גם הם.</span><span class="sxs-lookup"><span data-stu-id="ebb10-104">The client information is also logged.</span></span> <span data-ttu-id="ebb10-105">כך תוכל לזהות את כתובת ה-IP:</span><span class="sxs-lookup"><span data-stu-id="ebb10-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="ebb10-106">עבור אל [מרכז התאימות & אבטחה של Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="ebb10-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="ebb10-107">בחר חיפוש  >  **[ביומן הביקורת](https://go.microsoft.com/fwlink/?linkid=2103759)** של חיפוש.</span><span class="sxs-lookup"><span data-stu-id="ebb10-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="ebb10-108">אם אתה רואה הודעה שעליך להפעיל את הביקורת, הפעל אותה כעת.</span><span class="sxs-lookup"><span data-stu-id="ebb10-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="ebb10-109">אם תכונה זו אינה זמינה, תוצאות החיפוש לא יוכלו למשוך נתונים מתאריכים קודמים.</span><span class="sxs-lookup"><span data-stu-id="ebb10-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="ebb10-110">אם אתה מעוניין בפעילות ספציפית, בחר אותה מהרשימה **פעילויות** ; אחרת, כברירת מחדל, כל הפעילויות יוחזרו עבור המשתמש שנבחר.</span><span class="sxs-lookup"><span data-stu-id="ebb10-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="ebb10-111">שים לב שייתכן שפעילויות מסוימות לא יהיו זמינות לבחירה בתפריט ' **פעילויות** '; עם זאת, פריטי ביקורת אלה יוחזרו אם האפשרות ' הגדרת **תוצאות עבור כל הפעילויות** ' נבחרה (הגדרת ברירת המחדל).</span><span class="sxs-lookup"><span data-stu-id="ebb10-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="ebb10-112">ציין את טווח התאריכים, ובשדה **משתמשים** , בחר את שם המשתמש של המשתמש שברצונך לחקור.</span><span class="sxs-lookup"><span data-stu-id="ebb10-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="ebb10-113">בחר **חיפוש**.</span><span class="sxs-lookup"><span data-stu-id="ebb10-113">Select **Search**.</span></span> <span data-ttu-id="ebb10-114">הפעילויות מופיעות תחת **תוצאות**.</span><span class="sxs-lookup"><span data-stu-id="ebb10-114">The activities appear under **Results**.</span></span> <span data-ttu-id="ebb10-115">באפשרותך לראות את כתובת ה-IP עבור כל פעילות.</span><span class="sxs-lookup"><span data-stu-id="ebb10-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="ebb10-116">כדי להציג פרטים, בחר פעילות ולאחר מכן בחר **מידע נוסף**.</span><span class="sxs-lookup"><span data-stu-id="ebb10-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="ebb10-117">לקבלת מידע נוסף, ראה חיפוש [ביומן הביקורת של Office 365 כדי לפתור תרחישים נפוצים](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="ebb10-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>