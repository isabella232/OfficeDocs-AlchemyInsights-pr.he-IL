---
title: שימוש במניעת אובדן נתונים בכללי תעבורה
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915181"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="ca0e1-102">שימוש במניעת אובדן נתונים בכללי תעבורה</span><span class="sxs-lookup"><span data-stu-id="ca0e1-102">Using DLP in transport rules</span></span>

<span data-ttu-id="ca0e1-103">כדי לשלב מניעת אובדן נתונים (DLP) בתעבורה קיימת, השתמש בתנאי "**אם ההודעה מכילה... מידע רגיש**"בהגדרת כלל התעבורה.</span><span class="sxs-lookup"><span data-stu-id="ca0e1-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="ca0e1-104">**לקבלת פרטים נוספים, ראה:**</span><span class="sxs-lookup"><span data-stu-id="ca0e1-104">**For more details, see:**</span></span>

- <span data-ttu-id="ca0e1-105">שילוב מניעת אובדן סוגי נתונים רגישים בכללי תעבורה: [שלב כללי מידע רגישים](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="ca0e1-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="ca0e1-106">ניתן גם לבדוק את הכלל עם או ללא בדיקת מדיניות במצב בדיקה.</span><span class="sxs-lookup"><span data-stu-id="ca0e1-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="ca0e1-107">עליך להמתין 30 דקות לאחר יצירת הכלל לפני בדיקתו.</span><span class="sxs-lookup"><span data-stu-id="ca0e1-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="ca0e1-108">ראה [בדיקת כללי זרימת דואר/תעבורה](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="ca0e1-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="ca0e1-109">**שים לב**: אם אתה מנסה ליישם מדיניות מניעת אובדן נתונים חדשה באמצעות כללי תעבורה במרכז הניהול של Exchange (EAC), השתמש ב-[פריטי מדיניות מניעת אובדן נתונים במרכז האבטחה והתאימות](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="ca0e1-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
