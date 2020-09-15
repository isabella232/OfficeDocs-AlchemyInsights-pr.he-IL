---
title: יצירת הודעת דואר אלקטרוני לתפוס את כל
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712987"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="28f29-102">יצירת הודעת דואר אלקטרוני לתפוס את כל</span><span class="sxs-lookup"><span data-stu-id="28f29-102">Create an email catch all</span></span>

<span data-ttu-id="28f29-103">השימוש במלכוד כולו מבוטל מאוד.</span><span class="sxs-lookup"><span data-stu-id="28f29-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="28f29-104">מוטב לספק חזרה לשולח המאפשר לשולחים לדעת שאין אפשרות לשלוח את ההודעה שלהם ככתובת, כדי שיוכלו לפעול.</span><span class="sxs-lookup"><span data-stu-id="28f29-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="28f29-105">באפשרותך גם להגביל את תיבת הדואר המנוטר כדי ללכוד רק כתובות דואר אלקטרוני חוקיות בעבר.</span><span class="sxs-lookup"><span data-stu-id="28f29-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="28f29-106">כל תיבת דואר של כל מציאה תקבל הודעת דואר זבל מצויינת וייתכן שתתמלא בסופו של דבר אם לא יתבצע פיקוח מקרוב.</span><span class="sxs-lookup"><span data-stu-id="28f29-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="28f29-107">(קיימות מגבלות מתקבלות.)</span><span class="sxs-lookup"><span data-stu-id="28f29-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="28f29-108">אם תחליט להמשיך, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="28f29-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="28f29-109">יצירת קבוצת תפוצה דינאמית & כלול את כל סוגי הנמענים.</span><span class="sxs-lookup"><span data-stu-id="28f29-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="28f29-110">צור תיבת דואר ייעודית כדי לתפוס הודעות דואר אלקטרוני, לדוגמה, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="28f29-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="28f29-111">עבור התחום הספציפי, הגדר את DomainType "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="28f29-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="28f29-112">אם לאחר מכן תסיר את האפשרות תפוס הכל, הקפד להגדיר את התחום בחזרה לסמכותי.</span><span class="sxs-lookup"><span data-stu-id="28f29-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="28f29-113">צור כלל תעבורה של זרימת דואר באופן הבא:</span><span class="sxs-lookup"><span data-stu-id="28f29-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="28f29-114">אם השולח הוא "מחוץ לארגון"</span><span class="sxs-lookup"><span data-stu-id="28f29-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="28f29-115">ניתוב מחדש של ההודעה ל-Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="28f29-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="28f29-116">למעט אם הנמען הוא חבר ב-allusers@domain.com (קבוצת תפוצה מכילה את כל החברים)</span><span class="sxs-lookup"><span data-stu-id="28f29-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="28f29-117">הקפד לוודא שתיבות דואר חדשות נוספות לקבוצת התפוצה הדינאמית</span><span class="sxs-lookup"><span data-stu-id="28f29-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
