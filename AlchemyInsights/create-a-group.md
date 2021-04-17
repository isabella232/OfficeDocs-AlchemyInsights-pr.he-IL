---
title: יצירת קבוצה
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816357"
---
# <a name="create-a-group"></a><span data-ttu-id="5b73d-102">יצירת קבוצה</span><span class="sxs-lookup"><span data-stu-id="5b73d-102">Create a group</span></span>

<span data-ttu-id="5b73d-103">נושא זה מתאר יצירת קבוצה.</span><span class="sxs-lookup"><span data-stu-id="5b73d-103">This topic describes group creation.</span></span>

<span data-ttu-id="5b73d-104">**הרשאה ליצירת קבוצה**</span><span class="sxs-lookup"><span data-stu-id="5b73d-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="5b73d-105">ודא שאתה מורשה ליצור קבוצה חדשה.</span><span class="sxs-lookup"><span data-stu-id="5b73d-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="5b73d-106">מנהלי מערכת כלליים יכולים להפוך יצירת קבוצה ללא זמינה בפורטל Azure או Access ה- Panel.</span><span class="sxs-lookup"><span data-stu-id="5b73d-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="5b73d-107">ייתכן שתצטרך מנהל מערכת כדי ליצור את הקבוצה החדשה בשבילך, או כדי להעניק לך הרשאות מתאימות.</span><span class="sxs-lookup"><span data-stu-id="5b73d-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="5b73d-108">**ניהול הרשאות יצירת קבוצה**</span><span class="sxs-lookup"><span data-stu-id="5b73d-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="5b73d-109">מנהלי מערכת כלליים יכולים לנהל הרשאות יצירת קבוצות (מסיבות הקשורות לאבטחה) או קבוצות Office 365 שנוצרו בפורטל Azure או בלוח Access, על-ידי בחירה באפשרות "משתמשים יכולים ליצור קבוצות אבטחה בפורטלים של Azure" או "משתמשים יכולים ליצור קבוצות Office 365 בפורטלים של Azure" בכל הקבוצות  >  **הכלליות (הגדרות).**</span><span class="sxs-lookup"><span data-stu-id="5b73d-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="5b73d-110">באפשרותך גם להגביל יצירת קבוצה כדי לבחור קבוצת משתמשים אם יש לך רשיון Azure Active Directory P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="5b73d-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="5b73d-111">**הפיכת הודעת ברוך הבא ללא זמין עבור חברי הקבוצה החדשים של Office 365**</span><span class="sxs-lookup"><span data-stu-id="5b73d-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="5b73d-112">ניתן לבטל את הודעת הפתיחה שנשלחת למשתמשים שנוספו לקבוצות Office 365 על-ידי הגדרת **UnifiedGroupWelcomeMessageEnabled** ל- False ב- Powershell.</span><span class="sxs-lookup"><span data-stu-id="5b73d-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="5b73d-113">קבל מידע על הגדרה זו [כאן](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="5b73d-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

