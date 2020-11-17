---
title: יצירת קבוצה
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088903"
---
# <a name="create-a-group"></a><span data-ttu-id="d4209-102">יצירת קבוצה</span><span class="sxs-lookup"><span data-stu-id="d4209-102">Create a group</span></span>

<span data-ttu-id="d4209-103">נושא זה מתאר יצירת קבוצה.</span><span class="sxs-lookup"><span data-stu-id="d4209-103">This topic describes group creation.</span></span>

<span data-ttu-id="d4209-104">**הרשאה ליצירת קבוצה**</span><span class="sxs-lookup"><span data-stu-id="d4209-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="d4209-105">ודא שאתה מורשה ליצור קבוצה חדשה.</span><span class="sxs-lookup"><span data-stu-id="d4209-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="d4209-106">מנהלי מערכת כלליים יכולים להפוך את יצירת הקבוצה ללא זמינה בלוח תכלת או בלוח הגישה.</span><span class="sxs-lookup"><span data-stu-id="d4209-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="d4209-107">ייתכן שתזדקק למנהל מערכת כדי ליצור את הקבוצה החדשה עבורך, או כדי להעניק לך הרשאות מתאימות.</span><span class="sxs-lookup"><span data-stu-id="d4209-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="d4209-108">**ניהול הרשאות יצירת קבוצה**</span><span class="sxs-lookup"><span data-stu-id="d4209-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="d4209-109">מנהלי מערכת כלליים יכולים לנהל הרשאות יצירת קבוצה (למטרות הקשורות לאבטחה) או קבוצות של Office 365 שנוצרו בפורטל תכלת או ב-Access, על-ידי בחירה "משתמשים יכולים ליצור קבוצות אבטחה בפורטלים של תכלת" או "משתמשים יכולים ליצור קבוצות של office 365 בפורטלים של תכלת" בכל **הקבוצות**  >  **כללי (**</span><span class="sxs-lookup"><span data-stu-id="d4209-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="d4209-110">באפשרותך גם להגביל את יצירת הקבוצה כדי לבחור קבוצת משתמשים אם יש לך רשיון תכלת של Active Directory P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="d4209-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="d4209-111">**הפיכת הודעת הפתיחה ללא זמינה עבור חברים בקבוצה חדשה של Office 365**</span><span class="sxs-lookup"><span data-stu-id="d4209-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="d4209-112">ניתן להפוך את הודעת הפתיחה למשתמשים שנוספו לקבוצות של Office 365 לבלתי זמינה על-ידי הגדרת **UnifiedGroupWelcomeMessageEnabled** ל-False ב-Powershell.</span><span class="sxs-lookup"><span data-stu-id="d4209-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="d4209-113">קבל מידע על הגדרה זו [כאן](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="d4209-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

