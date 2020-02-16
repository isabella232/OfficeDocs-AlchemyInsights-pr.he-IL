---
title: הגדרות מדיניות פגישה
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042845"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="552cd-102">ניהול מדיניות פגישה בצוותי Microsoft</span><span class="sxs-lookup"><span data-stu-id="552cd-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="552cd-103">**הערה: ניתן לבצע עד 24 שעות כדי ששינויי מדיניות ייכנסו לתוקף עבור משתמשים.**</span><span class="sxs-lookup"><span data-stu-id="552cd-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="552cd-104">ייתכן שלא תוכל לבצע שינויים בפריטי מדיניות חדשים שנוצרו באופן מיידי; המתן 4 שעות ונסה לשנות שוב מדיניות חדשה שנוצרה.</span><span class="sxs-lookup"><span data-stu-id="552cd-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="552cd-105">מדיניות פגישה משמשת לשליטה בתכונות הזמינות לפגישה עם משתתפים בפגישות שתוזמנו על-ידי משתמשים בארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="552cd-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="552cd-106">ייתכן שחלק מהתכונות של מדיניות הפגישה לא יושמו במרכז הניהול של הצוותים עדיין (אלה מתויגים "בקרוב" בתיעוד).</span><span class="sxs-lookup"><span data-stu-id="552cd-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="552cd-107">במקרה זה, או אם אתה מקבל שגיאה כמו "אנחנו לא יכולים לעדכן את המדיניות עכשיו, אבל לנסות את זה שוב מאוחר יותר" במרכז הניהול של צוותי Microsoft, אנו ממליצים להשתמש ב-PowerShell כדי ליצור או לשנות מדיניות פגישה של צוותים.</span><span class="sxs-lookup"><span data-stu-id="552cd-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="552cd-108">לקבלת מידע נוסף אודות מדיניות פגישה, עיין במשאבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="552cd-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="552cd-109">כדי ללמוד אודות יצירת פריטי מדיניות, ביצוע שינויים והקצאת משתמשים למדיניות, ראה [ניהול מדיניות פגישה בצוותים](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="552cd-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="552cd-110">כדי לבצע שינויי מדיניות באמצעות יישומוני cmdlet PowerShell, ראה [קבוצות מבט כולל של powershell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="552cd-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="552cd-111">אתה צריך להשתמש [סקייפ עבור עסקים PowerShell מודול](https://www.microsoft.com/download/details.aspx?id=39366) עבור צוותי מדיניות פגישה.</span><span class="sxs-lookup"><span data-stu-id="552cd-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="552cd-112">בדוק את [התיעוד \*-c, מדיניות יישומוני ה-cmdlet](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="552cd-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

