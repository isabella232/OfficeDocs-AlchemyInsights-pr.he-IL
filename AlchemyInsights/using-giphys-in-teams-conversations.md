---
title: שימוש ב- Giphys Teams שיחות
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
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323521"
---
# <a name="using-giphys-in-teams-conversations"></a>שימוש ב- Giphys Teams שיחות

גישת Giphys בצ'Teams'אט זמינה כברירת מחדל. כמנהל מערכת, באפשרותך לקבוע אם Giphys זמין למשתמשים [על-ידי](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) הגדרת מדיניות העברת הודעות והבטחה שהשימוש ב- **Giphys בשיחות** הוא **ב-**.

אם קובצי GIF אינם פועלים כצפוי בשיחות Teams, ודא:

מדיניות [העברת ההודעות](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) צריכה לאפשר Giphys. כדי לאמת באמצעות כלי cmdlet של PowerShell:

- ודא ש באפשרותך לנהל [את Teams באמצעות PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- הפעל את הפקודה [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) וודא שהאפשרות **AllowGiphy** מוגדרת ל- **TRUE**.
- אם **AllowGiphy** מוגדר ל- **FALSE**, הפעל את הפקודה הבאה של PowerShell [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True.](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)

[יש להפוך חוויות](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) מחוברות אופציונליות לזמינות כדי לאפשר גישה לכתובת ה- URL של Giphy.

**הערה:** אם נקבעה לך מדיניות Teams העברת הודעות מרובות עבור הדייר שלך, באפשרותך לקבוע את זהות המדיניות שהוקצתה למשתמש מושפע באמצעות הפקודה [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | בחר TeamsMessagingPolicy.
