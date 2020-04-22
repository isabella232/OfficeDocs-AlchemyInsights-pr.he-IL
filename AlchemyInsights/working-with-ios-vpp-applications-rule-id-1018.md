---
title: עבודה עם iOS VPP חוק כלל מזהה 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719958"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="eebd2-102">עבודה עם iOS VPP יישומים</span><span class="sxs-lookup"><span data-stu-id="eebd2-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="eebd2-103">קרא [כיצד לנהל את האפליקציות iOS שנרכשו באמצעות תוכנית לרכישת אמצעי אחסון עם Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) כדי ללמוד אודות תכונות, אילוצים, ושלבים כדי לעשות שימוש בתוכנית הרכישה של אפל נפח ותמיכה עבור אותו ב-Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="eebd2-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="eebd2-104">**סוגיות נפוצות:** "הוצבתי app VPP iOS למשתמשים שלי, אבל ההתקנה נכשלה."</span><span class="sxs-lookup"><span data-stu-id="eebd2-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="eebd2-105">הדבר עלול לקרות אם אסימון VPP יחיד משמש באמצעות מספר ספקי ניהול התקנים ניידים מרובים.</span><span class="sxs-lookup"><span data-stu-id="eebd2-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="eebd2-106">אסימוני VPP מ-Apple יכולים לשמש רק עם ספק אחד.</span><span class="sxs-lookup"><span data-stu-id="eebd2-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="eebd2-107">אם השתמשת באסימון VPP עם ספקים מרובים, עליך להעלות מחדש את האסימון ל-Intune.</span><span class="sxs-lookup"><span data-stu-id="eebd2-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="eebd2-108">ההתקנה יכולה גם להיכשל אם המספר הכולל של ההתקנות חורג ממספר הרשיונות.</span><span class="sxs-lookup"><span data-stu-id="eebd2-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="eebd2-109">כדי להציג דוח שימוש עבור הרשיונות שלך, עבור אל דף \> **היישומים Intune Mobile** **App** .</span><span class="sxs-lookup"><span data-stu-id="eebd2-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="eebd2-110">כדי ללמוד כיצד להשיב רישיונות בשימוש, עיין [במאמר זה.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="eebd2-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
