---
title: 1491-חיפוש-לא-חוזר-צפוי-תוצאות
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510573"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="3c096-102">חיפוש תוכן לא מחזיר תוצאות צפויות</span><span class="sxs-lookup"><span data-stu-id="3c096-102">Content Search not returning expected results</span></span>

<span data-ttu-id="3c096-103">בעת הפעלת חיפושי תוכן מתוך מרכז התאימות של Microsoft 365 _ אמפר _, ייתכן שתקבל תוצאות חיפוש בלתי צפויות.</span><span class="sxs-lookup"><span data-stu-id="3c096-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="3c096-104">שקול את הדברים הבאים שיכולים להשפיע על תוצאות החיפוש שלך:</span><span class="sxs-lookup"><span data-stu-id="3c096-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="3c096-105">**מיקומי תוכן ותנאי חיפוש**: ודא שבחרת את מיקומי התוכן ותנאי החיפוש המתאימים.</span><span class="sxs-lookup"><span data-stu-id="3c096-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="3c096-106">אם הרצת חיפוש גדול (עם מיקומים רבים), שקול לפצל אותו לחיפושים מרובים.</span><span class="sxs-lookup"><span data-stu-id="3c096-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="3c096-107">**פריטים בעלי אינדקס חלקי**: פריטים בעלי [אינדקס חלקי](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) מתיבות דואר נכללים בתוצאות החיפוש המשוערות.</span><span class="sxs-lookup"><span data-stu-id="3c096-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="3c096-108">עם זאת, פריטים הכלולים באינדקס חלקי מאתרים ב-SharePoint ו-OneDrive אינם נכללים בהערכת החיפוש.</span><span class="sxs-lookup"><span data-stu-id="3c096-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="3c096-109">**כשלים בחיפוש**: בעת חיפוש במספר רב של תיבות דואר (מעל 100,000 תיבות דואר), ייתכן שתקבל שגיאות חיפוש, עם קודי שגיאה כגון CS008-009 ו-CS012-002).</span><span class="sxs-lookup"><span data-stu-id="3c096-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="3c096-110">במקרה זה, נסה שנית לבצע את החיפוש רק עבור מיקומי התוכן שנכשלו.</span><span class="sxs-lookup"><span data-stu-id="3c096-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="3c096-111">לקבלת מידע נוסף, עיין [במאמר זה](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="3c096-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
