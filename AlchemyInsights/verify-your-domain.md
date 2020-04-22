---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
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
ms.openlocfilehash: 2c4d8e075d2cf7214b5ef005b856daf7fb0ed53c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710444"
---
# <a name="verify-your-domain"></a><span data-ttu-id="9ed83-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="9ed83-102">Verify your domain</span></span>

 <span data-ttu-id="9ed83-103">**סביר להניח שהרשומה לא עודכנה ברחבי האינטרנט.**</span><span class="sxs-lookup"><span data-stu-id="9ed83-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="9ed83-104">זה בדרך כלל לוקח כמה דקות כדי שנוכל לראות את התקליט החדש, אבל לפעמים זה יכול להימשך כמה שעות.</span><span class="sxs-lookup"><span data-stu-id="9ed83-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="9ed83-105">אם חיכית כבר זמן כה רב, בדוק שהעתקת והדבקת את הערך המדויק ברשומת אימות TXT במארח ה-DNS שלך.</span><span class="sxs-lookup"><span data-stu-id="9ed83-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="9ed83-106">אחת הבעיות הנפוצות היא השמטה של חלק הרשומה "‎MS =‎".</span><span class="sxs-lookup"><span data-stu-id="9ed83-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="9ed83-107">אנו צריכים גם את החלק הזה!</span><span class="sxs-lookup"><span data-stu-id="9ed83-107">We need that too!</span></span>

- <span data-ttu-id="9ed83-108">אצל מארחי DNS מסוימים, עליך לבצע פעולה נוספת כדי לשמור את קובץ האזור (המקום שבו מאוחסנת רשומת ה- DNS) כך שהוא יתעדכן ברחבי האינטרנט.</span><span class="sxs-lookup"><span data-stu-id="9ed83-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="9ed83-109">ודא ששמרת את השינויים שלך כדי ש-Microsoft תוכל לראות ולאמת את הרשומה.</span><span class="sxs-lookup"><span data-stu-id="9ed83-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
