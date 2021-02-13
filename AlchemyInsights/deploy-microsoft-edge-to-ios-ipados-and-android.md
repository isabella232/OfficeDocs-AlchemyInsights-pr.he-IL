---
title: פריסת Microsoft Edge ל-iOS, iPadOS ו-Android
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8241"
- "9004604"
ms.openlocfilehash: 524e87ab57e29823361053093708c83831f19687
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194522"
---
# <a name="deploy-microsoft-edge-to-ios-ipados-and-android"></a><span data-ttu-id="7d6b6-102">פריסת Microsoft Edge ל-iOS, iPadOS ו-Android</span><span class="sxs-lookup"><span data-stu-id="7d6b6-102">Deploy Microsoft Edge to iOS, iPadOS, and Android</span></span>

<span data-ttu-id="7d6b6-103">התרחיש המודרך להלן יסייע לך להקצות את Microsoft Edge למשתמשים של מכשירי iOS, iPadOS ו-Android.</span><span class="sxs-lookup"><span data-stu-id="7d6b6-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span>

> [!NOTE]
> <span data-ttu-id="7d6b6-104">אם חסמת משתמשים לרשום מכשירים ניידים, תרחיש מודרך זה לא יפעל והמשתמשים יצטרכו להתקין את Microsoft Edge בעצמם.</span><span class="sxs-lookup"><span data-stu-id="7d6b6-104">If you blocked users from enrolling mobile devices, this guided scenario won't work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="7d6b6-105">התרחיש המודרך כולל את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="7d6b6-105">The guided scenario involves the following steps:</span></span>

1. [<span data-ttu-id="7d6b6-106">דרישות מוקדמות</span><span class="sxs-lookup"><span data-stu-id="7d6b6-106">Prerequisites</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#prerequisites)
2. [<span data-ttu-id="7d6b6-107">מבוא</span><span class="sxs-lookup"><span data-stu-id="7d6b6-107">Introduction</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-1---introduction)
3. [<span data-ttu-id="7d6b6-108">יסודות</span><span class="sxs-lookup"><span data-stu-id="7d6b6-108">Basics</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-2---basics)
4. [<span data-ttu-id="7d6b6-109">תצורה</span><span class="sxs-lookup"><span data-stu-id="7d6b6-109">Configuration</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-3---configuration)
5. [<span data-ttu-id="7d6b6-110">מטלות</span><span class="sxs-lookup"><span data-stu-id="7d6b6-110">Assignments</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-4---assignments)
6. [<span data-ttu-id="7d6b6-111">סקירה ויצירה</span><span class="sxs-lookup"><span data-stu-id="7d6b6-111">Review and creation</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-5---review--create)

<span data-ttu-id="7d6b6-112">לאחר השלמת השלבים בתרחיש המודרך, מדיניות ההתאמה של Microsoft intune תאפשר את התכונות הבאות של Microsoft Edge for business:</span><span class="sxs-lookup"><span data-stu-id="7d6b6-112">After you complete the steps in the guided scenario, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="7d6b6-113">זהות כפולה</span><span class="sxs-lookup"><span data-stu-id="7d6b6-113">Dual identity</span></span>
- <span data-ttu-id="7d6b6-114">שילוב עם מדיניות הגנת היישומים של Microsoft intune</span><span class="sxs-lookup"><span data-stu-id="7d6b6-114">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="7d6b6-115">שילוב עם Proxy של היישום ' תכלת Active Directory '</span><span class="sxs-lookup"><span data-stu-id="7d6b6-115">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="7d6b6-116">קיצורי מועדפים ודפי בית מנוהלים</span><span class="sxs-lookup"><span data-stu-id="7d6b6-116">Managed favorites and home page shortcuts</span></span>
