---
title: 1332 OWA - הכללים של תיבת הדואר הנכנס לא מבצעים עבור תיבת דואר
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f090d0a9d84bc6a4d1a1f4c0af55102d4b0ddfbe
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29472777"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="0a833-102">כלל תיבת הדואר הנכנס אינו פועל כצפוי</span><span class="sxs-lookup"><span data-stu-id="0a833-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="0a833-103">אמת את ההגדרות הבאות:</span><span class="sxs-lookup"><span data-stu-id="0a833-103">Verify the following settings:</span></span>
  
- <span data-ttu-id="0a833-p101">הודעה ניתן לנתב מחדש, העברה או שהשיבו עליהן באופן אוטומטי בהתבסס על כללי תיבת דואר נכנס פעם אחת בלבד. מנתב מחדש כלל (כלל תיבת דואר נכנס או כלל זרימת דואר, המכונה גם כלל התעבורה) ניתן להוסיף מספר מרבי של נמענים העברה עשרה הודעה. לקבלת מידע נוסף, ראה [מגבלות כלל יומן, תעבורה, ואת תיבת הדואר הנכנס](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="0a833-p101">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time. A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message. For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>
    
- <span data-ttu-id="0a833-p102">כללי תיבת דואר נכנס אינם פועלים רישום חלופי בתיבת הדואר. לקבלת מידע נוסף אודות תיבת הדואר רישום חלופי, ראה [תיבת הדואר של רישום ביומן חלופי](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="0a833-p102">Inbox rules don't work on the alternate journaling mailbox. For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>
    
<span data-ttu-id="0a833-109">כדי לפתור בעיות אלה, ראה [2829319 קילו -בתים](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="0a833-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>
  
<span data-ttu-id="0a833-110">אם לא תחיל הבעיות הקודמת, הפעל את הדוח האבחון כלל תיבת דואר נכנס לפני הפנה לגורם בכיר יותר של הבעיה למחלקת התמיכה של Microsoft:</span><span class="sxs-lookup"><span data-stu-id="0a833-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>
  
1. <span data-ttu-id="0a833-111">פתח את תיבת הדואר שלך ב- Outlook באינטרנט ולאחר מכן לחץ על **הגדרות** \> **אפשרויות** \> **דואר אלקטרוני של ארגון** \> **כללי תיבת דואר נכנס**.</span><span class="sxs-lookup"><span data-stu-id="0a833-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>
    
2. <span data-ttu-id="0a833-112">בחלק התחתון של הדף, לחץ על **אם הכללים שלך אינם פועלים על לחץ כאן כדי להפיק את הדוח האבחון**.</span><span class="sxs-lookup"><span data-stu-id="0a833-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
    

