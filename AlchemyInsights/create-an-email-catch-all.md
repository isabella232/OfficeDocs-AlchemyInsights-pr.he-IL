---
title: ליצור דוא ל לתפוס את כל
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286194"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="2f455-102">ליצור דוא ל לתפוס את כל</span><span class="sxs-lookup"><span data-stu-id="2f455-102">Create an email catch all</span></span>

<span data-ttu-id="2f455-103">השימוש במלכוד מאוד מיואש.</span><span class="sxs-lookup"><span data-stu-id="2f455-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="2f455-104">מוטב לספק חזרה לשולח כדי ששולחים יידעו שההודעה שלהם לא הועברה כממוענות כדי שיוכלו לפעול.</span><span class="sxs-lookup"><span data-stu-id="2f455-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="2f455-105">אתה יכול גם להגביל את תיבת הדואר בפיקוח לתפוס רק בעבר כתובות דוא ל חוקיים.</span><span class="sxs-lookup"><span data-stu-id="2f455-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="2f455-106">כל לתפוס את כל תיבת הדואר יקבל הרבה דואר זבל והוא עשוי בסופו של דבר למלא אם לא פיקוח צמוד.</span><span class="sxs-lookup"><span data-stu-id="2f455-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="2f455-107">(קיימים מגבלות מתקבלות.)</span><span class="sxs-lookup"><span data-stu-id="2f455-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="2f455-108">אם תחליט להמשיך, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="2f455-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="2f455-109">צור קבוצת תפוצה דינאמית _ אמפר _ כלול את "כל סוגי הנמענים".</span><span class="sxs-lookup"><span data-stu-id="2f455-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="2f455-110">צור תיבת דואר ייעודית לתפיסת הודעות דוא ל, לדוגמה, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="2f455-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="2f455-111">עבור התחום הספציפי, הגדר את הDomainType ל' ממסר הפנמה '.</span><span class="sxs-lookup"><span data-stu-id="2f455-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="2f455-112">אם מאוחר יותר תסיר את כל המלכוד, הקפד להגדיר את התחום בחזרה לסמכותי.</span><span class="sxs-lookup"><span data-stu-id="2f455-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="2f455-113">צור כלל תעבורת דואר אלקטרוני באופן הבא:</span><span class="sxs-lookup"><span data-stu-id="2f455-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="2f455-114">אם השולח הוא "מחוץ לארגון"</span><span class="sxs-lookup"><span data-stu-id="2f455-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="2f455-115">נתב מחדש את ההודעה לCatchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="2f455-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="2f455-116">אלא אם הנמען חבר ב-allusers@domain.com (קבוצת הפצה מכילה את כל החברים)</span><span class="sxs-lookup"><span data-stu-id="2f455-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="2f455-117">הקפד לאמת שתיבות דואר חדשות יתווספו לקבוצת ההפצה הדינאמית</span><span class="sxs-lookup"><span data-stu-id="2f455-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
