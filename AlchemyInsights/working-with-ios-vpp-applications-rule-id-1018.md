---
title: עבודה עם iOS VPP יישומים כלל מזהה 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 65b9a727171a7551068717f6327f15e1aa8e6bed
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420485"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="265c9-102">עבודה עם iOS יישומים VPP</span><span class="sxs-lookup"><span data-stu-id="265c9-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="265c9-103">קרא [כיצד לנהל יישומים iOS שנרכשו באמצעות תוכנית רכישה בכמות עם Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) כדי ללמוד אודות התכונות, אילוצים השלבים כדי להפוך להשתמש של תוכנית רכישה של אמצעי האחסון תפוח ותמיכה עבור אותו ב- Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="265c9-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="265c9-104">**בעיות נפוצות:** "להקצות יישום VPP iOS המשתמשים שלי, אך ההתקנה נכשלה".</span><span class="sxs-lookup"><span data-stu-id="265c9-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="265c9-105">הדבר יכול לקרות אם נעשה שימוש ב- token VPP יחיד על-פני מספר ספקים ניהול של מכשיר נייד.</span><span class="sxs-lookup"><span data-stu-id="265c9-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="265c9-106">ניתן להשתמש באסימונים VPP מ- Apple רק עם ספק אחד.</span><span class="sxs-lookup"><span data-stu-id="265c9-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="265c9-107">אם השתמשת אסימון VPP עם ספקים מרובים, עליך לטעון מחדש את האסימון כדי Intune.</span><span class="sxs-lookup"><span data-stu-id="265c9-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="265c9-108">ההתקנה עלול להיכשל גם אם המספר הכולל של התקנות לחרוג ממספר הרשיונות.</span><span class="sxs-lookup"><span data-stu-id="265c9-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="265c9-109">כדי להציג של הדוח שימוש עבור הרישיונות שלך, עבור אל **apps ניידים Intune** \> דף **רשיונות App** .</span><span class="sxs-lookup"><span data-stu-id="265c9-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="265c9-110">כדי ללמוד כיצד לפנות רשיונות בשימוש, עיין [מאמר זה.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="265c9-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

