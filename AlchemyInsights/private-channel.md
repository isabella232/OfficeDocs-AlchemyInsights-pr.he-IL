---
title: ערוץ פרטי
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005439"
---
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="97536-102">ערוצים פרטיים בצוותי Microsoft</span><span class="sxs-lookup"><span data-stu-id="97536-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="97536-103">ערוצים פרטיים הם תכונה חדשה בצוותי Microsoft.</span><span class="sxs-lookup"><span data-stu-id="97536-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="97536-104">שים לב שאין אפשרות להמיר ערוצים פרטיים מערוצים רגילים או להיפך.</span><span class="sxs-lookup"><span data-stu-id="97536-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="97536-105">לקבלת פרטים אודות ערוצים פרטיים, כגון מידע אודות [יצירת ערוצים פרטיים ואתרי](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) [SharePoint של ערוצים](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)פרטיים, ראה [ערוצים פרטיים בצוותי Microsoft](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span><span class="sxs-lookup"><span data-stu-id="97536-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="97536-106">**הערה:** מאחר שתצורה עבור שמירה של הודעות ערוץ פרטי אינה נתמכת עדיין, לדיירים עם מדיניות שמירה מאופשרת לא יהיו ערוצים פרטיים הזמינים כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="97536-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="97536-107">ניתן להפעיל ערוצים פרטיים במרכז הניהול של הצוותים.</span><span class="sxs-lookup"><span data-stu-id="97536-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="97536-108">בנוסף, שים לב שבזמן שמירה של הודעות ערוץ פרטי אינה נתמכת, קיימת תמיכה בשמירה של קבצים המשותפים בערוצים פרטיים.</span><span class="sxs-lookup"><span data-stu-id="97536-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="97536-109">**צריך בעל צוות חדש?**</span><span class="sxs-lookup"><span data-stu-id="97536-109">**Need a new team owner?**</span></span>

<span data-ttu-id="97536-110">אם בעל הערוץ הפרטי שלך עוזב, באפשרותך להוסיף בעל צוות חדש דרך צוותי Powershell.</span><span class="sxs-lookup"><span data-stu-id="97536-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="97536-111">לך [לכאן](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) כדי להתקין את הצוותים Powershell.</span><span class="sxs-lookup"><span data-stu-id="97536-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="97536-112">להלן יישומון ה-cmdlet הדרוש לך:</span><span class="sxs-lookup"><span data-stu-id="97536-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="97536-113">לקבלת מידע נוסף על צוותי Powershell, ראה [קבוצות מבט כולל על powershell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="97536-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>
