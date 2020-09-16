---
title: 1491-חיפוש-לא-חוזר-התוצאות הצפויות
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
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740475"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="0d4d6-102">חיפוש תוכן אינו מחזיר תוצאות צפויות</span><span class="sxs-lookup"><span data-stu-id="0d4d6-102">Content Search not returning expected results</span></span>

<span data-ttu-id="0d4d6-103">בעת הפעלת חיפושי תוכן ממרכז התאימות של Microsoft 365 security &, ייתכן שתקבל תוצאות חיפוש בלתי צפויות.</span><span class="sxs-lookup"><span data-stu-id="0d4d6-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="0d4d6-104">שקול את הדברים הבאים העשויים להשפיע על תוצאות החיפוש:</span><span class="sxs-lookup"><span data-stu-id="0d4d6-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="0d4d6-105">**מיקומים ותנאי חיפוש של תוכן**: ודא שבחרת את מיקומי התוכן המתאימים ותנאי חיפוש.</span><span class="sxs-lookup"><span data-stu-id="0d4d6-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="0d4d6-106">אם הפעלת חיפוש גדול (עם מיקומים רבים), שקול לפצל אותו לחיפושים מרובים.</span><span class="sxs-lookup"><span data-stu-id="0d4d6-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="0d4d6-107">**פריטים הכלולים באינדקס באופן חלקי**: פריטים הכלולים  [באינדקס באופן חלקי](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) מתיבות דואר כלולים בתוצאות החיפוש המוערכות.</span><span class="sxs-lookup"><span data-stu-id="0d4d6-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="0d4d6-108">עם זאת, פריטים הכלולים באינדקס באופן חלקי מאתרים ב-SharePoint ו-OneDrive אינם כלולים בהערכת החיפוש.</span><span class="sxs-lookup"><span data-stu-id="0d4d6-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="0d4d6-109">**כשלים בחיפוש**: בעת חיפוש מספר גדול של תיבות דואר (מעל לתיבות דואר של 100,000), אתה עשוי לקבל שגיאות חיפוש, עם קודי שגיאה כגון CS008-900 ו-CS012-002).</span><span class="sxs-lookup"><span data-stu-id="0d4d6-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="0d4d6-110">במקרה זה, נסה שוב לבצע את החיפוש עבור מיקומי התוכן שכשלו.</span><span class="sxs-lookup"><span data-stu-id="0d4d6-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="0d4d6-111">עיין  [במאמר זה](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="0d4d6-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
