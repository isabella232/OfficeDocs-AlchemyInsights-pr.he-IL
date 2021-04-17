---
title: הגדרות מדיניות פגישה
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
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825444"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="a5bd1-102">ניהול מדיניות פגישה ב- Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="a5bd1-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="a5bd1-103">**הערה: שינויים במדיניות ייכנסו לתוקף עבור המשתמשים עד 24 שעות.**</span><span class="sxs-lookup"><span data-stu-id="a5bd1-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="a5bd1-104">ייתכן שלא תוכל לבצע שינויים במדיניות חדשה שנוצרה באופן מיידי; המתן 4 שעות ותנסי שוב לשנות מדיניות חדשה שנוצרה.</span><span class="sxs-lookup"><span data-stu-id="a5bd1-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="a5bd1-105">מדיניות פגישה משמשת לשליטה בתכונות הזמינות למשתתפי הפגישה עבור פגישות המתוזמנות על-ידי משתמשים בארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="a5bd1-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="a5bd1-106">ייתכן שתכונות מסוימות של מדיניות פגישה עדיין לא יושמו במרכז הניהול של Teams (אלה מסומנות כ"בקרוב" בתיעוד).</span><span class="sxs-lookup"><span data-stu-id="a5bd1-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="a5bd1-107">במקרה זה, או אם אתה מקבל שגיאה כמו "אין לנו אפשרות לעדכן את המדיניות כעת, אך נסה אותה שוב מאוחר יותר" במרכז הניהול של Microsoft Teams, מומלץ להשתמש ב- PowerShell כדי ליצור או לשנות את מדיניות הפגישה של Teams.</span><span class="sxs-lookup"><span data-stu-id="a5bd1-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="a5bd1-108">לקבלת מידע נוסף אודות מדיניות פגישה, עיין במשאבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="a5bd1-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="a5bd1-109">כדי ללמוד אודות יצירת פריטי מדיניות, ביצוע שינויים והקצאת משתמשים למדיניות, ראה [ניהול מדיניות פגישה ב- Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="a5bd1-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="a5bd1-110">כדי לבצע שינויי מדיניות באמצעות כלי cmdlet של PowerShell, ראה [מבט כולל על Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="a5bd1-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="a5bd1-111">עליך להשתמש במודול [Skype for Business PowerShell עבור](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) פריטי מדיניות פגישה של Teams.</span><span class="sxs-lookup"><span data-stu-id="a5bd1-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="a5bd1-112">עיין [בתיעוד ה- cmdlets של \*-CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="a5bd1-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

