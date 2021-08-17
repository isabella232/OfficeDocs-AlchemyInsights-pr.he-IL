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
ms.openlocfilehash: 0244b68ffa2ebd3d70bae66a24ac299004848557b63b17c2ea74fafaff22bb8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104309"
---
# <a name="using-giphys-in-teams-conversations"></a>שימוש ב- Giphys Teams שיחות

גישת Giphys בצ'Teams'אט זמינה כברירת מחדל. כמנהל מערכת, באפשרותך לקבוע אם Giphys זמין למשתמשים [על-ידי](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) הגדרת מדיניות העברת הודעות והבטחה שהשימוש ב- **Giphys בשיחות** הוא **ב-**.

אם קובצי GIF אינם פועלים כצפוי בשיחות Teams, ודא:

מדיניות [העברת ההודעות](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) צריכה לאפשר Giphys. כדי לאמת באמצעות כלי cmdlet של PowerShell:

- ודא ש באפשרותך לנהל [את Teams באמצעות PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- הפעל את הפקודה [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) וודא שהאפשרות **AllowGiphy** מוגדרת ל- **TRUE**.
- אם **AllowGiphy** מוגדר ל- **FALSE**, הפעל את הפקודה הבאה של PowerShell [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True.](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)

[יש להפוך חוויות](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) מחוברות אופציונליות לזמינות כדי לאפשר גישה לכתובת ה- URL של Giphy.

> [!NOTE]
> אם יש לך מדיניות Teams העברת הודעות מרובות המוגדרת עבור הדייר שלך, באפשרותך לקבוע את זהות המדיניות שהוקצתה למשתמש המושפע באמצעות הפקודה [PowerShell Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | בחר TeamsMessagingPolicy.
