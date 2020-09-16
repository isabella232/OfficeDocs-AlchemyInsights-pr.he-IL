---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734307"
---
# <a name="verify-your-domain"></a><span data-ttu-id="81f42-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="81f42-102">Verify your domain</span></span>

 <span data-ttu-id="81f42-103">**כנראה שהרשומה לא עודכנה לאורך האינטרנט.**</span><span class="sxs-lookup"><span data-stu-id="81f42-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="81f42-104">בדרך כלל נדרשות רק כמה דקות כדי שנוכל לראות את הרשומה החדשה, אך לעתים היא עשויה להימשך זמן רב מספר שעות.</span><span class="sxs-lookup"><span data-stu-id="81f42-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="81f42-105">אם כבר חיכית כל-כך הרבה זמן, בדוק שוב שהעתקת והדבקת את הערך המדויק ברשומת אימות ה-TXT אצל מארח ה-DNS שלך.</span><span class="sxs-lookup"><span data-stu-id="81f42-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="81f42-106">אחת הבעיות הנפוצות היא השמטה של חלק הרשומה "‎MS =‎".</span><span class="sxs-lookup"><span data-stu-id="81f42-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="81f42-107">אנו צריכים גם את החלק הזה!</span><span class="sxs-lookup"><span data-stu-id="81f42-107">We need that too!</span></span>

- <span data-ttu-id="81f42-108">אצל מארחי DNS מסוימים, עליך לבצע פעולה נוספת כדי לשמור את קובץ האזור (המקום שבו מאוחסנת רשומת ה- DNS) כך שהוא יתעדכן ברחבי האינטרנט.</span><span class="sxs-lookup"><span data-stu-id="81f42-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="81f42-109">ודא ששמרת את השינויים כך ש-Microsoft תוכל לראות את הרשומה ולאמת אותה.</span><span class="sxs-lookup"><span data-stu-id="81f42-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
