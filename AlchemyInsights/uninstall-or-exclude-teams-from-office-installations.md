---
title: הסרת התקנה או אי-Teams מהתקנות Office ההתקנה
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
- "2662"
- "9000660"
ms.openlocfilehash: a960c96abf6215e3a34908ce8669a0c61298daac829343b3673dbfef0c4cbfc7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007719"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>הסרת התקנה או Teams הוצאה מהתקנות חדשות או Office קיימות

Microsoft Teams נכלל כחלק מ- יישומי Microsoft 365 לארגונים, יישומי Microsoft 365 לעסקים ו- Office עבור Mac.

- השתמש בכלי [Office הפריסה כדי](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) לא לכלול Teams התקנות חדשות של Office.
- כדי *להסיר* Teams התקנה ממכשיר שבו פועל Windows, ראה [הסרת Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). כדי לנקות Microsoft Teams מחשבים או משתמשים מרובים של יעד, [ראה ניקוי Microsoft Teams פריסה.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)
- השתמש באפשרות [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) כדי למנוע Microsoft Teams התקנה אוטומטית באמצעות Office.
- השתמש באפשרות [PreventFirstLaunchAfterInstall,](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) *לפני Teams*, כדי למנוע הפעלה Microsoft Teams אוטומטית לאחר ההתקנה.

אם אתה משתמש ב- Office עבור Mac, [ראה Microsoft Teams התקנות ב- Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).