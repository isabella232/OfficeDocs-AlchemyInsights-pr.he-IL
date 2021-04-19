---
title: שימוש במניעת אובדן נתונים בכללי תעבורה
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827217"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="58b34-102">שימוש במניעת אובדן נתונים בכללי תעבורה</span><span class="sxs-lookup"><span data-stu-id="58b34-102">Using DLP in transport rules</span></span>

<span data-ttu-id="58b34-103">כדי לשלב מניעת אובדן נתונים (DLP) בתעבורה קיימת, השתמש בתנאי "**אם ההודעה מכילה... מידע רגיש**"בהגדרת כלל התעבורה.</span><span class="sxs-lookup"><span data-stu-id="58b34-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="58b34-104">**לקבלת פרטים נוספים, ראה:**</span><span class="sxs-lookup"><span data-stu-id="58b34-104">**For more details, see:**</span></span>

- <span data-ttu-id="58b34-105">שילוב מניעת אובדן סוגי נתונים רגישים בכללי תעבורה: [שלב כללי מידע רגישים](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="58b34-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="58b34-106">ניתן גם לבדוק את הכלל עם או ללא בדיקת מדיניות במצב בדיקה.</span><span class="sxs-lookup"><span data-stu-id="58b34-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="58b34-107">עליך להמתין 30 דקות לאחר יצירת הכלל לפני בדיקתו.</span><span class="sxs-lookup"><span data-stu-id="58b34-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="58b34-108">ראה [בדיקת כללי זרימת דואר/תעבורה](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="58b34-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="58b34-109">**שים לב**: אם אתה מנסה ליישם מדיניות מניעת אובדן נתונים חדשה באמצעות כללי תעבורה במרכז הניהול של Exchange (EAC), השתמש ב-[פריטי מדיניות מניעת אובדן נתונים במרכז האבטחה והתאימות](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="58b34-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
