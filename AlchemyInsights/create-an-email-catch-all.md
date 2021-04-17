---
title: יצירת הודעת דואר אלקטרוני תופסת הכל
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816201"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="2799c-102">יצירת הודעת דואר אלקטרוני תופסת הכל</span><span class="sxs-lookup"><span data-stu-id="2799c-102">Create an email catch all</span></span>

<span data-ttu-id="2799c-103">השימוש במלכוד אינו מיואש במיוחד.</span><span class="sxs-lookup"><span data-stu-id="2799c-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="2799c-104">עדיף לספק קפיצה חזרה לשולח, כך ששולחים יודעים שלא היתה אפשרות להעביר את ההודעה שלהם ככתובת כך שהם יכולים לבצע פעולה.</span><span class="sxs-lookup"><span data-stu-id="2799c-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="2799c-105">באפשרותך גם להגביל את תיבת הדואר המנוהלת כדי לתפוס רק כתובות דואר אלקטרוני חוקיות בעבר.</span><span class="sxs-lookup"><span data-stu-id="2799c-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="2799c-106">כל תפיסה של כל תיבת הדואר תקבל עסקה טובה של דואר זבל, ובסופו של דבר עשויה למלא אותה אם לא תנטר אותה מקרוב.</span><span class="sxs-lookup"><span data-stu-id="2799c-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="2799c-107">(ישנם מגבלות קבלה.)</span><span class="sxs-lookup"><span data-stu-id="2799c-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="2799c-108">אם תחליט להמשיך, בצע את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="2799c-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="2799c-109">יצירת קבוצת תפוצה דינאמית & "כל סוגי הנמענים".</span><span class="sxs-lookup"><span data-stu-id="2799c-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="2799c-110">צור תיבת דואר ייעודית כדי לתפוס הודעות דואר אלקטרוני, לדוגמה, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="2799c-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="2799c-111">עבור התחום הספציפי, הגדר את DomainType ל- "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="2799c-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="2799c-112">אם תסיר מאוחר יותר את התלכוד הכל, הקפד להגדיר את התחום בחזרה ל'סמכותי'.</span><span class="sxs-lookup"><span data-stu-id="2799c-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="2799c-113">צור כלל תעבורה של זרימת דואר באופן הבא:</span><span class="sxs-lookup"><span data-stu-id="2799c-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="2799c-114">אם השולח הוא "מחוץ לארגון"</span><span class="sxs-lookup"><span data-stu-id="2799c-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="2799c-115">ניתוב מחדש של ההודעה Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="2799c-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="2799c-116">למעט אם הנמען חבר ב- allusers@domain.com (קבוצת תפוצה מכילה את כל החברים)</span><span class="sxs-lookup"><span data-stu-id="2799c-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="2799c-117">ודא כי תיבות דואר חדשות מתווספות לקבוצת התפוצה הדינאמית</span><span class="sxs-lookup"><span data-stu-id="2799c-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
