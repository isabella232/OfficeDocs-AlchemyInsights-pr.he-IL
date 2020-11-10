---
title: שימוש ב-Giphys בשיחות Teams
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982508"
---
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="6323c-102">שימוש ב-Giphys בשיחות Teams</span><span class="sxs-lookup"><span data-stu-id="6323c-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="6323c-103">Giphys access ב-Teams chat מופעל כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="6323c-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="6323c-104">כמנהל מערכת, באפשרותך לקבוע אם Giphys זמינים למשתמשים על-ידי [הגדרת מדיניות העברת הודעות](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) והבטחת **השימוש ב-Giphys בשיחות** **מופעל**.</span><span class="sxs-lookup"><span data-stu-id="6323c-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="6323c-105">אם קבצי Gif אינם פועלים כמצופה בשיחות Teams, ודא:</span><span class="sxs-lookup"><span data-stu-id="6323c-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="6323c-106">[מדיניות העברת ההודעות](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) צריכה לאפשר Giphys.</span><span class="sxs-lookup"><span data-stu-id="6323c-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="6323c-107">כדי לאמת באמצעות רכיבי cmdlet של PowerShell:</span><span class="sxs-lookup"><span data-stu-id="6323c-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="6323c-108">ודא שבאפשרותך [לנהל צוותים באמצעות PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="6323c-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="6323c-109">הפעיל את הפקודה PowerShell [Get-CsTeamsMessagingPolicy-Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) וודא ש- **AllowGiphy** מוגדר ל- **TRUE**.</span><span class="sxs-lookup"><span data-stu-id="6323c-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="6323c-110">אם **AllowGiphy** מוגדר ל- **FALSE** , הפעלת ערכת הפקודות הבאה של PowerShell- [CsTeamsMessagingPolicy-Identity Global-AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="6323c-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="6323c-111">יש להפוך [חוויות מקושרות אופציונליות](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) לזמינות כדי לאפשר גישה לכתובת ה-URL של Giphy.</span><span class="sxs-lookup"><span data-stu-id="6323c-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="6323c-112">אם מוגדרות מספר מדיניות העברת הודעות של Teams עבור הדייר שלך, באפשרותך לקבוע את זהות המדיניות שהוקצתה למשתמש המושפע באמצעות הפקודה PowerShell [-Get-CsOnlineUser-identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | בחר TeamsMessagingPolicy.</span><span class="sxs-lookup"><span data-stu-id="6323c-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
