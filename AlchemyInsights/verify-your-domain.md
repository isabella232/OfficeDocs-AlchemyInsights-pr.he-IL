---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51770992"
---
# <a name="verify-your-domain"></a><span data-ttu-id="c0c11-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="c0c11-102">Verify your domain</span></span>

 <span data-ttu-id="c0c11-103">**סביר להניח שההקלטה לא עודכנה ברחבי האינטרנט.**</span><span class="sxs-lookup"><span data-stu-id="c0c11-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="c0c11-104">בדרך כלל נדרשות כמה דקות בלבד כדי שנוכל לראות את הרשומה החדשה, אך מדי פעם זה יכול נמשכת כמה שעות.</span><span class="sxs-lookup"><span data-stu-id="c0c11-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="c0c11-105">אם כבר חיכית זמן זה, בדוק שוב שהעתקת והדבקת את הערך המדויק ברשומת אימות TXT במארח ה- DNS שלך.</span><span class="sxs-lookup"><span data-stu-id="c0c11-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="c0c11-106">אחת הבעיות הנפוצות היא השמטה של חלק הרשומה "‎MS =‎".</span><span class="sxs-lookup"><span data-stu-id="c0c11-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="c0c11-107">אנו צריכים גם את החלק הזה!</span><span class="sxs-lookup"><span data-stu-id="c0c11-107">We need that too!</span></span>

- <span data-ttu-id="c0c11-108">אצל מארחי DNS מסוימים, עליך לבצע פעולה נוספת כדי לשמור את קובץ האזור (המקום שבו מאוחסנת רשומת ה- DNS) כך שהוא יתעדכן ברחבי האינטרנט.</span><span class="sxs-lookup"><span data-stu-id="c0c11-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="c0c11-109">ודא ששמרת את השינויים שלך כדי ש- Microsoft תוכל לראות ולאמת את הרשומה.</span><span class="sxs-lookup"><span data-stu-id="c0c11-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
