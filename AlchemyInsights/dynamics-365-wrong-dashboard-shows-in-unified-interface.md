---
title: Dynamics 365-מציג לוח שגוי ב-Dynamics 365 ממשק אחיד
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/25/2019
ms.locfileid: "36528552"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="9dfd1-102">מופעי לוח מחוונים שגויים בממשק מאוחד של Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="9dfd1-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="9dfd1-103">קיימות מספר סיבות לכך שניתן לראות לוח מחוונים אחר מאשר האחד שציפית לו:</span><span class="sxs-lookup"><span data-stu-id="9dfd1-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="9dfd1-104">המשתמש הגדיר לוח מחוונים של ברירת מחדל למשתמש</span><span class="sxs-lookup"><span data-stu-id="9dfd1-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="9dfd1-105">בדרך כלל באפשרותך לזהות לוח מחוונים של ברירת מחדל של משתמש מוגדר אם הלחצן **קבע כברירת מחדל** אינו מופיע בשורת הפקודה של לוח המחוונים.</span><span class="sxs-lookup"><span data-stu-id="9dfd1-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="9dfd1-106">לוח המחוונים המוגדר כברירת מחדל של המשתמש יעקוף את כל לוחות המחוונים האחרים המהווים ברירת מחדל, גם אם מחוונים ברירת המחדל של המשתמש אינם נמצאים ביישום</span><span class="sxs-lookup"><span data-stu-id="9dfd1-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="9dfd1-107">השתמש במעקף הבא כדי לבטל את הגדרת לוח המחוונים שלהם.</span><span class="sxs-lookup"><span data-stu-id="9dfd1-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="9dfd1-108">צור לוח מחוונים אישי חדש.</span><span class="sxs-lookup"><span data-stu-id="9dfd1-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="9dfd1-109">הגדר את לוח המחוונים החדש כברירת המחדל של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="9dfd1-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="9dfd1-110">. תמחק את לוח המחוונים</span><span class="sxs-lookup"><span data-stu-id="9dfd1-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="9dfd1-111">לוח המחוונים ממוקם במפת האתר</span><span class="sxs-lookup"><span data-stu-id="9dfd1-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="9dfd1-112">ייתכן שהגדרת לוח מחוונים של ברירת מחדל של ארגון על-ידי בחירת לוח מחוונים ובחירה באפשרות ' קבע כברירת מחדל ' תחת ' התאמה אישית של המערכת '.</span><span class="sxs-lookup"><span data-stu-id="9dfd1-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="9dfd1-113">אבל לוח המחוונים המוגדר במעצב מפת האתר יקבל קדימות על פני לוח מחוונים זה, אם למשתמש יש גישה אליו.</span><span class="sxs-lookup"><span data-stu-id="9dfd1-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="9dfd1-114">כדי שהמשתמשים יראו את לוח המחוונים שהגדרת כברירת המחדל של הארגון, באפשרותך:</span><span class="sxs-lookup"><span data-stu-id="9dfd1-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="9dfd1-115">הגדר את לוח המחוונים במפת האתר</span><span class="sxs-lookup"><span data-stu-id="9dfd1-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="9dfd1-116">הסר את הגישה ללוח המחוונים המוגדר על מפת האתר עבור אותם משתמשים</span><span class="sxs-lookup"><span data-stu-id="9dfd1-116">Remove access to the sitemap defined dashboard for those users</span></span>
