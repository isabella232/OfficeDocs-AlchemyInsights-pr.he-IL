---
title: 1332 כללי תיבת הדואר הנכנס (s) אינם מבצעים עבור תיבת דואר
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9abdcdcb33d39b8b9fe2df80f0c15a8b55e465fd
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44576561"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="ce592-102">כלל תיבת דואר נכנס אינו פועל כמצופה</span><span class="sxs-lookup"><span data-stu-id="ce592-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="ce592-103">בדוק את ההגדרות הבאות ב-Outlook באינטרנט:</span><span class="sxs-lookup"><span data-stu-id="ce592-103">Verify the following settings in Outlook on the web:</span></span>

- <span data-ttu-id="ce592-104">ניתן לנתב מחדש הודעה, להעביר אותה או להשיבו באופן אוטומטי בהתבסס על כללי תיבת הדואר הנכנס רק פעם אחת.</span><span class="sxs-lookup"><span data-stu-id="ce592-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="ce592-105">כלל מכוון מחודש (כלל תיבת דואר נכנס או כלל זרימת דואר, הידוע גם ככלל תעבורה) יכול להוסיף להודעה מקסימום עשרה נמעני העברה.</span><span class="sxs-lookup"><span data-stu-id="ce592-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="ce592-106">לקבלת מידע נוסף, ראה [מגבלות כלל של יומן, תעבורה ותיבת דואר נכנס](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="ce592-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="ce592-107">כללי תיבת דואר נכנס אינם פועלים בתיבת הדואר של הרישום החלופי.</span><span class="sxs-lookup"><span data-stu-id="ce592-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="ce592-108">לקבלת מידע נוסף אודות תיבת הדואר החלופית לרישום ביומן, ראה [תיבת דואר חלופית לרישום ביומן](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="ce592-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="ce592-109">כדי לפתור בעיות אלה, ראה [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="ce592-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="ce592-110">אם הבעיות הקודמות אינן חלות, הפעל את דוח האבחון של כלל תיבת הדואר הנכנס לפני שאתה מהחריף את הבעיה לתמיכת Microsoft:</span><span class="sxs-lookup"><span data-stu-id="ce592-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="ce592-111">פתח את תיבת הדואר ב-Outlook באינטרנט ולחץ על</span><span class="sxs-lookup"><span data-stu-id="ce592-111">Open the mailbox in Outlook on the web, and click</span></span> <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 <span data-ttu-id="ce592-112">**הגדרות**  >  **הצג את כל הגדרות Outlook**  >  **Mail**  >  **כללים**.</span><span class="sxs-lookup"><span data-stu-id="ce592-112">**Settings** > **View all Outlook Settings** > **Mail** > **Rules**.</span></span>

2. <span data-ttu-id="ce592-113">בתחתית הדף, לחץ על **אם הכללים שלך אינם פועלים לחץ כאן כדי ליצור דוח אבחון**.</span><span class="sxs-lookup"><span data-stu-id="ce592-113">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
