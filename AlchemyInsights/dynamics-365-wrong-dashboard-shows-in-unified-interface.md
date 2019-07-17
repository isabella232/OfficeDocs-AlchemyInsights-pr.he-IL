---
title: Dynamics 365 - לוח מחוונים של שגוי מציגה ממשק מאוחד Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 6edf6fbae0174f3fa4d635c7a99e7daae1243b60
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/16/2019
ms.locfileid: "35747779"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="f6b22-102">לוח מחוונים של שגוי מציגה ממשק מאוחד Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="f6b22-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="f6b22-103">קיימות מספר סיבות לכך רואה לוח מחוונים אחר מזה שאתה מצפה:</span><span class="sxs-lookup"><span data-stu-id="f6b22-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="f6b22-104">המשתמש הגדיר לוח מחוונים של משתמש המהווה ברירת מחדל</span><span class="sxs-lookup"><span data-stu-id="f6b22-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="f6b22-105">בדרך כלל תוכל לזהות משתמש המחוונים המהווה ברירת מחדל נקבע אם לחצן **קבע כברירת מחדל** תציג בשורת הפקודה של לוח מחוונים.</span><span class="sxs-lookup"><span data-stu-id="f6b22-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="f6b22-106">המחוונים המהווה ברירת מחדל של המשתמש יעקוף כל אחרים ברירת מחדל לוחות מחוונים, גם אם המחוונים המהווה ברירת מחדל של המשתמש אינו ב- app הנוכחי.</span><span class="sxs-lookup"><span data-stu-id="f6b22-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="f6b22-107">השתמש הדרך הבאה לעקיפת הבעיה כדי ביטול קביעה של סיסמת המחוונים המהווה ברירת מחדל שלהם.</span><span class="sxs-lookup"><span data-stu-id="f6b22-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="f6b22-108">צור לוח מחוונים אישי חדש.</span><span class="sxs-lookup"><span data-stu-id="f6b22-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="f6b22-109">הגדרת לוח מחוונים חדש זה כברירת המחדל של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="f6b22-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="f6b22-110">מחיקת לוח מחוונים זה.</span><span class="sxs-lookup"><span data-stu-id="f6b22-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="f6b22-111">לוח המחוונים מוגדר במפת אתר</span><span class="sxs-lookup"><span data-stu-id="f6b22-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="f6b22-112">ייתכן שהגדרת את המחוונים המהווה ברירת מחדל של הארגון על-ידי בחירת לוח מחוונים ובחירה באפשרות 'קבע כברירת מחדל' תחת 'התאמה אישית של המערכת'.</span><span class="sxs-lookup"><span data-stu-id="f6b22-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="f6b22-113">אך לוח המחוונים שהוגדרו מעצב sitemap יקבלו קדימות על פני לוח מחוונים זה, אם למשתמש יש גישה אליו.</span><span class="sxs-lookup"><span data-stu-id="f6b22-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="f6b22-114">כדי לגרום למשתמשים לראות את לוח המחוונים שהגדרת כברירת המחדל של הארגון, באפשרותך:</span><span class="sxs-lookup"><span data-stu-id="f6b22-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="f6b22-115">הגדרת לוח מחוונים זה במפת אתר</span><span class="sxs-lookup"><span data-stu-id="f6b22-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="f6b22-116">הסר גישה ללוח המחוונים sitemap שהוגדרו עבור משתמשים אלה</span><span class="sxs-lookup"><span data-stu-id="f6b22-116">Remove access to the sitemap defined dashboard for those users</span></span>
