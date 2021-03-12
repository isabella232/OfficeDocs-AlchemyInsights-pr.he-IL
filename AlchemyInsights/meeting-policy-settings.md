---
title: הגדרות מדיניות פגישה
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
- "9000734"
- "2657"
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704607"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="9c4ad-102">ניהול מדיניות פגישה ב-Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="9c4ad-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="9c4ad-103">**הערה: אפשרות זו יכולה להימשך עד 24 שעות כדי ששינויי מדיניות ייכנסו לתוקף עבור משתמשים.**</span><span class="sxs-lookup"><span data-stu-id="9c4ad-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="9c4ad-104">ייתכן שלא תוכל לבצע שינויים בפריטי מדיניות חדשים שנוצרו באופן מיידי; המתן 4 שעות ונסה לשנות מדיניות חדשה שנוצרה שוב.</span><span class="sxs-lookup"><span data-stu-id="9c4ad-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="9c4ad-105">פריטי מדיניות של פגישה משמשים לשליטה בתכונות הזמינות למשתתפים בפגישה לפגישות המתוזמנות על-ידי משתמשים בארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="9c4ad-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="9c4ad-106">ייתכן שתכונות מסוימות של פריטי מדיניות פגישה לא יושמו במרכז הניהול של Teams עדיין (אלה מסומנות "בקרוב" בתיעוד).</span><span class="sxs-lookup"><span data-stu-id="9c4ad-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="9c4ad-107">במקרה זה, או אם אתה מקבל שגיאה כגון "לא ניתן לעדכן את המדיניות כעת, אך נסה שוב מאוחר יותר" במרכז הניהול של Microsoft Teams, מומלץ להשתמש ב-PowerShell כדי ליצור או לשנות מדיניות של פגישות של Teams.</span><span class="sxs-lookup"><span data-stu-id="9c4ad-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="9c4ad-108">לקבלת מידע נוסף אודות מדיניות פגישה, עיין במשאבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="9c4ad-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="9c4ad-109">כדי ללמוד אודות יצירת מדיניות, ביצוע שינויים והקצאת משתמשים למדיניות, ראה [ניהול מדיניות פגישה ב-teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="9c4ad-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="9c4ad-110">כדי לבצע שינויים במדיניות באמצעות רכיבי cmdlet של PowerShell, ראה [מבט כולל על teams powershell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="9c4ad-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="9c4ad-111">עליך להשתמש במודול מדיניות הפגישה של [Skype For Business PowerShell](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) עבור teams.</span><span class="sxs-lookup"><span data-stu-id="9c4ad-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="9c4ad-112">סקור את [התיעוד של ' רכיבי cmdlet של CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="9c4ad-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

