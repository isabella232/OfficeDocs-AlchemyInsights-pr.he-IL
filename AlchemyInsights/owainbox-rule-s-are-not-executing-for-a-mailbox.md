---
title: 1332 OWA - הכללים של תיבת הדואר הנכנס לא מבצעים עבור תיבת דואר
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 901237d4dc7b99695097142c61a4bfef7c09750d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36555774"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="858f2-102">כלל תיבת הדואר הנכנס אינו פועל כצפוי</span><span class="sxs-lookup"><span data-stu-id="858f2-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="858f2-103">אמת את ההגדרות הבאות ב- Outlook באינטרנט:</span><span class="sxs-lookup"><span data-stu-id="858f2-103">Verify the following settings in Outlook on the web:</span></span>

- <span data-ttu-id="858f2-104">הודעה ניתן לנתב מחדש, העברה או שהשיבו עליהן באופן אוטומטי בהתבסס על כללי תיבת דואר נכנס פעם אחת בלבד.</span><span class="sxs-lookup"><span data-stu-id="858f2-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="858f2-105">מנתב מחדש כלל (כלל תיבת דואר נכנס או כלל זרימת דואר, המכונה גם כלל התעבורה) ניתן להוסיף מספר מרבי של נמענים העברה עשרה הודעה.</span><span class="sxs-lookup"><span data-stu-id="858f2-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="858f2-106">לקבלת מידע נוסף, ראה [מגבלות כלל יומן, תעבורה, ואת תיבת הדואר הנכנס](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="858f2-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="858f2-107">כללי תיבת דואר נכנס אינם פועלים רישום חלופי בתיבת הדואר.</span><span class="sxs-lookup"><span data-stu-id="858f2-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="858f2-108">לקבלת מידע נוסף אודות תיבת הדואר רישום חלופי, ראה [תיבת הדואר של רישום ביומן חלופי](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="858f2-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="858f2-109">כדי לפתור בעיות אלה, ראה [2829319 קילו -בתים](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="858f2-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="858f2-110">אם לא תחיל הבעיות הקודמת, הפעל את הדוח האבחון כלל תיבת דואר נכנס לפני הפנה לגורם בכיר יותר של הבעיה למחלקת התמיכה של Microsoft:</span><span class="sxs-lookup"><span data-stu-id="858f2-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="858f2-111">פתח את תיבת הדואר שלך ב- Outlook באינטרנט ולאחר מכן לחץ</span><span class="sxs-lookup"><span data-stu-id="858f2-111">Open the mailbox in Outlook on the web, and click</span></span> <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 <span data-ttu-id="858f2-112">**הגדרות** > **להציג את כל הגדרות Outlook** > **דואר** > **כללי**.</span><span class="sxs-lookup"><span data-stu-id="858f2-112">**Settings** > **View all Outlook Settings** > **Mail** > **Rules**.</span></span>

2. <span data-ttu-id="858f2-113">בחלק התחתון של הדף, לחץ על **אם הכללים שלך אינם פועלים על לחץ כאן כדי להפיק את הדוח האבחון**.</span><span class="sxs-lookup"><span data-stu-id="858f2-113">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
