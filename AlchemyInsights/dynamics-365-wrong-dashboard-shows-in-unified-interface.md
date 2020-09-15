---
title: דינמיקה של 365-לוח מחוונים שגוי מוצג בממשק המאוחד של Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711276"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="dccc6-102">לוח מחוונים שגוי מוצג בממשק המאוחד של Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="dccc6-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="dccc6-103">קיימות כמה סיבות לכך שאתה עשוי לראות לוח מחוונים שונה מזה שאתה מצפה לו:</span><span class="sxs-lookup"><span data-stu-id="dccc6-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="dccc6-104">המשתמש הגדיר לוח מחוונים המהווה ברירת מחדל של משתמש</span><span class="sxs-lookup"><span data-stu-id="dccc6-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="dccc6-105">בדרך כלל, באפשרותך לזהות לוח מחוונים המהווה ברירת מחדל של משתמש מוגדר אם הלחצן **קבע כברירת מחדל** אינו מוצג בסרגל הפקודות של לוח המחוונים.</span><span class="sxs-lookup"><span data-stu-id="dccc6-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="dccc6-106">לוח המחוונים המשמש כברירת מחדל של המשתמש יעקוף את כל לוחות המחוונים האחרים המהווים ברירת מחדל, גם אם לוח המחוונים המוגדר כברירת מחדל של המשתמש</span><span class="sxs-lookup"><span data-stu-id="dccc6-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="dccc6-107">השתמש בפתרון הבא כדי לבטל את הגדרת לוח המחוונים של ברירת המחדל.</span><span class="sxs-lookup"><span data-stu-id="dccc6-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="dccc6-108">יצירת לוח מחוונים אישי חדש.</span><span class="sxs-lookup"><span data-stu-id="dccc6-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="dccc6-109">הגדר את לוח המחוונים החדש כברירת מחדל של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="dccc6-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="dccc6-110">מחק לוח מחוונים זה.</span><span class="sxs-lookup"><span data-stu-id="dccc6-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="dccc6-111">לוח המחוונים מוגדר במפת האתר</span><span class="sxs-lookup"><span data-stu-id="dccc6-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="dccc6-112">ייתכן שהגדרת לוח מחוונים המשמש כברירת מחדל של ארגון על-ידי בחירת לוח מחוונים ובחירה באפשרות ' קבע כברירת מחדל ' תחת ' התאמה אישית של המערכת '.</span><span class="sxs-lookup"><span data-stu-id="dccc6-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="dccc6-113">אולם לוח המחוונים המוגדר במעצב מפת האתר יקבל קדימות על-פני לוח מחוונים זה, אם למשתמש יש גישה אליו.</span><span class="sxs-lookup"><span data-stu-id="dccc6-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="dccc6-114">כדי שמשתמשים יראו את לוח המחוונים שהגדרת כברירת המחדל של הארגון, תוכל לבצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="dccc6-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="dccc6-115">הגדרת לוח מחוונים זה במפת האתר</span><span class="sxs-lookup"><span data-stu-id="dccc6-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="dccc6-116">הסרת גישה ללוח המחוונים המוגדר על-ידי sitemap עבור משתמשים אלה</span><span class="sxs-lookup"><span data-stu-id="dccc6-116">Remove access to the sitemap defined dashboard for those users</span></span>
