---
title: 1332 OWA - הכללים של תיבת הדואר הנכנס לא מבצעים עבור תיבת דואר
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: c0b221b5335254bd0f1eb4b258efa6946376ca12
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/13/2019
ms.locfileid: "31858745"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="c3891-102">כלל תיבת הדואר הנכנס אינו פועל כצפוי</span><span class="sxs-lookup"><span data-stu-id="c3891-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="c3891-103">אמת את ההגדרות הבאות:</span><span class="sxs-lookup"><span data-stu-id="c3891-103">Verify the following settings:</span></span>

- <span data-ttu-id="c3891-104">הודעה ניתן לנתב מחדש, העברה או שהשיבו עליהן באופן אוטומטי בהתבסס על כללי תיבת דואר נכנס פעם אחת בלבד.</span><span class="sxs-lookup"><span data-stu-id="c3891-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="c3891-105">מנתב מחדש כלל (כלל תיבת דואר נכנס או כלל זרימת דואר, המכונה גם כלל התעבורה) ניתן להוסיף מספר מרבי של נמענים העברה עשרה הודעה.</span><span class="sxs-lookup"><span data-stu-id="c3891-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="c3891-106">לקבלת מידע נוסף, ראה [מגבלות כלל יומן, תעבורה, ואת תיבת הדואר הנכנס](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="c3891-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="c3891-107">כללי תיבת דואר נכנס אינם פועלים רישום חלופי בתיבת הדואר.</span><span class="sxs-lookup"><span data-stu-id="c3891-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="c3891-108">לקבלת מידע נוסף אודות תיבת הדואר רישום חלופי, ראה [תיבת הדואר של רישום ביומן חלופי](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="c3891-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="c3891-109">כדי לפתור בעיות אלה, ראה [2829319 קילו -בתים](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="c3891-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="c3891-110">אם לא תחיל הבעיות הקודמת, הפעל את הדוח האבחון כלל תיבת דואר נכנס לפני הפנה לגורם בכיר יותר של הבעיה למחלקת התמיכה של Microsoft:</span><span class="sxs-lookup"><span data-stu-id="c3891-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="c3891-111">פתח את תיבת הדואר שלך ב- Outlook באינטרנט ולאחר מכן לחץ על **הגדרות** \> **אפשרויות** \> **דואר אלקטרוני של ארגון** \> **כללי תיבת דואר נכנס**.</span><span class="sxs-lookup"><span data-stu-id="c3891-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>

2. <span data-ttu-id="c3891-112">בחלק התחתון של הדף, לחץ על **אם הכללים שלך אינם פועלים על לחץ כאן כדי להפיק את הדוח האבחון**.</span><span class="sxs-lookup"><span data-stu-id="c3891-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
