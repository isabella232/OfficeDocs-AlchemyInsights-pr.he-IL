---
title: עבודה עם iOS VPP Applications Rule Id 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688947"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="29eb1-102">עבודה עם יישומים של iOS VPP</span><span class="sxs-lookup"><span data-stu-id="29eb1-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="29eb1-103">קרא [כיצד לנהל יישומי iOS שנרכשו באמצעות תוכנית לרכישת נפח עם Microsoft intune](https://docs.microsoft.com/intune/vpp-apps-ios) כדי ללמוד אודות תכונות, אילוצים ושלבים לביצוע השימוש בתוכנית לרכישת נפח של Apple והתמיכה בה ב-Microsoft intune.</span><span class="sxs-lookup"><span data-stu-id="29eb1-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="29eb1-104">**בעיות נפוצות:** "הוצבתי אפליקציית iOS VPP למשתמשים שלי, אך ההתקנה נכשלה."</span><span class="sxs-lookup"><span data-stu-id="29eb1-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="29eb1-105">פעולה זו עשויה להתרחש אם אסימון אחד של VPP נמצא בשימוש בין ספקי ניהול מכשירים ניידים מרובים.</span><span class="sxs-lookup"><span data-stu-id="29eb1-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="29eb1-106">ניתן להשתמש באסימונים של VPP מ-Apple רק עם ספק אחד.</span><span class="sxs-lookup"><span data-stu-id="29eb1-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="29eb1-107">אם השתמשת באסימון VPP עם ספקים מרובים, עליך להעלות מחדש את האסימון לכיוון המנגינה.</span><span class="sxs-lookup"><span data-stu-id="29eb1-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="29eb1-108">ההתקנה יכולה גם להיכשל אם מספר ההתקנות הכולל חורג ממספר הרשיונות.</span><span class="sxs-lookup"><span data-stu-id="29eb1-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="29eb1-109">כדי להציג דוח שימוש עבור הרשיונות שלך, עבור לדף רשיונות האפליקציה ' **כוונון אפליקציות למכשירים ניידים** ' \> **App licenses** .</span><span class="sxs-lookup"><span data-stu-id="29eb1-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="29eb1-110">כדי ללמוד כיצד להחזיר רשיונות בשימוש, עיין [במאמר זה.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="29eb1-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
