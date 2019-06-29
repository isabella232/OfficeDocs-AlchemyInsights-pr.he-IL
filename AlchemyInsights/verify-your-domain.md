---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 5bd6c32a246db9dfcdb475368ade0441df4dc9c3
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365418"
---
# <a name="verify-your-domain"></a><span data-ttu-id="7b187-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="7b187-102">Verify your domain</span></span>

 <span data-ttu-id="7b187-103">**לעדכן את הרשומה ככל הנראה לא ברחבי האינטרנט.**</span><span class="sxs-lookup"><span data-stu-id="7b187-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="7b187-104">הוא בדרך כלל רק נמשך דקות אחדות עבורנו שניתן יהיה לראות את הרשומה החדשה, אך לעתים הוא יכול להימשך מספר שעות.</span><span class="sxs-lookup"><span data-stu-id="7b187-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="7b187-105">אם יצרת שהמתנת אשר כבר זמן רב, בדוק שוב כי אתה כבר העתקתי והדבקתי את הערך המדויק לתוך רשומת אימות ה-TXT במחשב מארח DNS שלך.</span><span class="sxs-lookup"><span data-stu-id="7b187-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="7b187-106">אחת הבעיות הנפוצות היא השמטה של חלק הרשומה "‎MS =‎".</span><span class="sxs-lookup"><span data-stu-id="7b187-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="7b187-107">אנו צריכים גם את החלק הזה!</span><span class="sxs-lookup"><span data-stu-id="7b187-107">We need that too!</span></span>

- <span data-ttu-id="7b187-108">אצל מארחי DNS מסוימים, עליך לבצע פעולה נוספת כדי לשמור את קובץ האזור (המקום שבו מאוחסנת רשומת ה- DNS) כך שהוא יתעדכן ברחבי האינטרנט.</span><span class="sxs-lookup"><span data-stu-id="7b187-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="7b187-109">הקפד לשמור את השינויים, כך ש- Office 365 יוכל לראות ולאמת את הרשומה.</span><span class="sxs-lookup"><span data-stu-id="7b187-109">Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
