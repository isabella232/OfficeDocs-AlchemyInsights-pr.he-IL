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
# <a name="using-giphys-in-teams-conversations"></a>שימוש ב-Giphys בשיחות Teams

Giphys access ב-Teams chat מופעל כברירת מחדל. כמנהל מערכת, באפשרותך לקבוע אם Giphys זמינים למשתמשים על-ידי [הגדרת מדיניות העברת הודעות](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) והבטחת **השימוש ב-Giphys בשיחות** **מופעל**.

אם קבצי Gif אינם פועלים כמצופה בשיחות Teams, ודא:

[מדיניות העברת ההודעות](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) צריכה לאפשר Giphys. כדי לאמת באמצעות רכיבי cmdlet של PowerShell:

- ודא שבאפשרותך [לנהל צוותים באמצעות PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- הפעיל את הפקודה PowerShell [Get-CsTeamsMessagingPolicy-Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) וודא ש- **AllowGiphy** מוגדר ל- **TRUE**.
- אם **AllowGiphy** מוגדר ל- **FALSE** , הפעלת ערכת הפקודות הבאה של PowerShell- [CsTeamsMessagingPolicy-Identity Global-AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

יש להפוך [חוויות מקושרות אופציונליות](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) לזמינות כדי לאפשר גישה לכתובת ה-URL של Giphy.

> [!NOTE]
> אם מוגדרות מספר מדיניות העברת הודעות של Teams עבור הדייר שלך, באפשרותך לקבוע את זהות המדיניות שהוקצתה למשתמש המושפע באמצעות הפקודה PowerShell [-Get-CsOnlineUser-identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | בחר TeamsMessagingPolicy.
