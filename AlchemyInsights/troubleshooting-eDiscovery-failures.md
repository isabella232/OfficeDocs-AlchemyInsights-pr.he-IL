---
title: 1490-פתרון בעיות-גילוי אלקטרוני-כשלים
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277842"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="cc96d-102">פתרון בעיות של שגיאות חיפוש תוכן</span><span class="sxs-lookup"><span data-stu-id="cc96d-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="cc96d-103">האם אתה נתקל בבעיות בחיפוש תוכן או מקבל כשלונות בעת ייצוא תוצאות חיפוש?</span><span class="sxs-lookup"><span data-stu-id="cc96d-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="cc96d-104">לדוגמה, האם אתה מקבל את הפרטים הבאים בעת הפעלת חיפושים?</span><span class="sxs-lookup"><span data-stu-id="cc96d-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="cc96d-105">שגיאות CS008 או CS012</span><span class="sxs-lookup"><span data-stu-id="cc96d-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="cc96d-106">שגיאות ' עסוק ' בשרת/פסק זמן</span><span class="sxs-lookup"><span data-stu-id="cc96d-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="cc96d-107">אירעה שגיאת יישום</span><span class="sxs-lookup"><span data-stu-id="cc96d-107">Application error occurred</span></span>

<span data-ttu-id="cc96d-108">לחלופין, כאשר אתה מחפש או מייצא תוצאות ממספר גדול של תיבות דואר (מעל לתיבות דואר של 100,000), האם אתה מקבל שגיאות ייצוא?</span><span class="sxs-lookup"><span data-stu-id="cc96d-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="cc96d-109">עבור סוגים אלה של שגיאות, נסה שוב לחפש את מיקומי התוכן שנכשלו.</span><span class="sxs-lookup"><span data-stu-id="cc96d-109">For these types of errors, retry the search for the content locations that have failed.</span></span> <span data-ttu-id="cc96d-110">עיין  [במאמר זה](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="cc96d-110">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="cc96d-111">אם אתה מייצא יותר מ-100 תיבות דואר, יהיה עליך להשתמש ב-Powershell הבאים כדי להוריד את תוצאות הייצוא:  [ייצוא תוצאות של יותר מ-100 תיבות דואר](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="cc96d-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
