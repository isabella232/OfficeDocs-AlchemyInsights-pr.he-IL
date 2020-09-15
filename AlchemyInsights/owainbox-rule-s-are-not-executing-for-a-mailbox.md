---
title: כללי OWA-Inbox של 1332 אינם מתבצעים עבור תיבת דואר
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f4d8db9c590abc490f193ef54a8a1dc5afba82b9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721592"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="e87f1-102">כלל תיבת דואר נכנס אינו פועל כמצופה</span><span class="sxs-lookup"><span data-stu-id="e87f1-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="e87f1-103">אמת את ההגדרות הבאות ב-Outlook באינטרנט:</span><span class="sxs-lookup"><span data-stu-id="e87f1-103">Verify the following settings in Outlook on the web:</span></span>

- <span data-ttu-id="e87f1-104">ניתן לנתב מחדש הודעה, להעביר או לקבל הודעה באופן אוטומטי בהתבסס על כללי תיבת דואר נכנס רק פעם אחת.</span><span class="sxs-lookup"><span data-stu-id="e87f1-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="e87f1-105">כלל ניתוב מחדש (כלל תיבת דואר נכנס או כלל זרימת דואר, הידוע גם ככלל תעבורה) יכול להוסיף להודעה עשרה נמעני העברה לכל היותר.</span><span class="sxs-lookup"><span data-stu-id="e87f1-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="e87f1-106">לקבלת מידע נוסף, ראה [מגבלות כללי של יומן, תעבורה ותיבת דואר נכנס](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="e87f1-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="e87f1-107">כללי תיבת דואר נכנס אינם פועלים בתיבת הדואר של הרישום החלופי.</span><span class="sxs-lookup"><span data-stu-id="e87f1-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="e87f1-108">לקבלת מידע נוסף אודות תיבת הדואר החלופית של רישום ביומן, ראה [תיבת דואר של רישום לסירוגין](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="e87f1-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="e87f1-109">כדי לפתור בעיות אלה, ראה [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="e87f1-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="e87f1-110">אם הבעיות הקודמות אינן חלות, הפעלת דוח אבחון כלל תיבת הדואר הנכנס לפני שאתה מחמיר את הבעיה עם התמיכה של Microsoft:</span><span class="sxs-lookup"><span data-stu-id="e87f1-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="e87f1-111">פתח את תיבת הדואר ב-Outlook באינטרנט ולחץ על</span><span class="sxs-lookup"><span data-stu-id="e87f1-111">Open the mailbox in Outlook on the web, and click</span></span> <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 <span data-ttu-id="e87f1-112">**הגדרות**  >  **הצגת כל הגדרות Outlook**  >  **דואר אלקטרוני**  >  **כללים**.</span><span class="sxs-lookup"><span data-stu-id="e87f1-112">**Settings** > **View all Outlook Settings** > **Mail** > **Rules**.</span></span>

2. <span data-ttu-id="e87f1-113">בחלק התחתון של הדף, לחץ על **אם הכללים שלך אינם פועלים לחץ כאן כדי ליצור דוח אבחון**.</span><span class="sxs-lookup"><span data-stu-id="e87f1-113">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
