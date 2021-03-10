---
title: החלת שיטות עבודה מומלצות עבור שאילתות ציד מתקדמות
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694273"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="0977f-102">החלת שיטות עבודה מומלצות עבור שאילתות ציד מתקדמות</span><span class="sxs-lookup"><span data-stu-id="0977f-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="0977f-103">כדי לקבל תוצאות במהירות רבה יותר וכדי להימנע מפסקי זמן בעת הפעלת שאילתות מורכבות, החל שיטות עבודה מומלצות אלה:</span><span class="sxs-lookup"><span data-stu-id="0977f-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="0977f-104">בעת ניסיון שאילתות חדשות, השתמש תמיד במגבלה, כדי להימנע מקבלת ערכות תוצאות גדולות מאוד.</span><span class="sxs-lookup"><span data-stu-id="0977f-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="0977f-105">כמו כן, השתמש `count` כדי לבצע הערכה ראשונית של גודל ערכת התוצאות.</span><span class="sxs-lookup"><span data-stu-id="0977f-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="0977f-106">השתמש תחילה במסנני זמן.</span><span class="sxs-lookup"><span data-stu-id="0977f-106">Use time filters first.</span></span> <span data-ttu-id="0977f-107">באופן אידיאלי, הגבל את השאילתות שלך לשבעה ימים.</span><span class="sxs-lookup"><span data-stu-id="0977f-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="0977f-108">בתחילת שאילתה, מיד לאחר המסנן ' שעה ', הוסף את המסננים הצפויים להסרת רוב הנתונים.</span><span class="sxs-lookup"><span data-stu-id="0977f-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="0977f-109">בעת חיפוש אסימונים מלאים, השתמש `has` באופרטור במקום באופרטור `contains` .</span><span class="sxs-lookup"><span data-stu-id="0977f-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="0977f-110">הפעל חיפוש בעמודה ספציפית במקום בכל העמודות.</span><span class="sxs-lookup"><span data-stu-id="0977f-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="0977f-111">בעת הצטרפות לטבלאות, ציין תחילה את הטבלה עם פחות שורות.</span><span class="sxs-lookup"><span data-stu-id="0977f-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="0977f-112">`project` רק את העמודות הדרושות מהטבלאות שצירפת.</span><span class="sxs-lookup"><span data-stu-id="0977f-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="0977f-113">לקבלת מידע נוסף, ראה [שיטות עבודה מומלצות לשאילתות ציד מתקדמות](https://go.microsoft.com/fwlink/?linkid=2144812).</span><span class="sxs-lookup"><span data-stu-id="0977f-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
