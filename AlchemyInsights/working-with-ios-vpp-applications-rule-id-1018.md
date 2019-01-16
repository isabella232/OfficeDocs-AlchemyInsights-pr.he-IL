---
title: עבודה עם iOS VPP יישומים כלל מזהה 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 5bcfb6dd7222bd102ff2620c19bfb943e7bd9591
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28292813"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="f8e56-102">עבודה עם iOS יישומים VPP</span><span class="sxs-lookup"><span data-stu-id="f8e56-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="f8e56-103">קרא [כיצד לנהל יישומים iOS שנרכשו באמצעות תוכנית רכישה בכמות עם Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) כדי ללמוד אודות התכונות, אילוצים השלבים כדי להפוך להשתמש של תוכנית רכישה של אמצעי האחסון תפוח ותמיכה עבור אותו ב- Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="f8e56-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="f8e56-104">**בעיות נפוצות:** "להקצות יישום VPP iOS המשתמשים שלי, אך ההתקנה נכשלה".</span><span class="sxs-lookup"><span data-stu-id="f8e56-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="f8e56-p101">הדבר יכול לקרות אם נעשה שימוש ב- token VPP יחיד על-פני מספר ספקים ניהול של מכשיר נייד. ניתן להשתמש באסימונים VPP מ- Apple רק עם ספק אחד. אם השתמשת אסימון VPP עם ספקים מרובים, עליך לטעון מחדש את האסימון כדי Intune.</span><span class="sxs-lookup"><span data-stu-id="f8e56-p101">This can happen if a single VPP token is used across multiple mobile device management providers. VPP tokens from Apple may only be used with one provider. If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="f8e56-p102">ההתקנה עלול להיכשל גם אם המספר הכולל של התקנות לחרוג ממספר הרשיונות. כדי להציג של הדוח שימוש עבור הרישיונות שלך, עבור אל **apps ניידים Intune** \> דף **רשיונות App** . כדי ללמוד כיצד לפנות רשיונות בשימוש, עיין [מאמר זה.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="f8e56-p102">The installation can also fail if the total number of installations exceed the number of licenses. To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page. To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

