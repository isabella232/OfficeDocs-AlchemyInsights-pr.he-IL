---
title: הסרת התקנה או אי הכללה של Teams מהתקנות Office
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
- "2662"
- "9000660"
ms.openlocfilehash: 22d69db749671afdfe7a809d1bc598e2ad1891d8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658222"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>הסרת התקנה או אי-הכללה של Teams מהתקנות חדשות או קיימות של Office

Microsoft Teams כלול כחלק מ-Microsoft 365 Apps עבור enterprise, יישומי Microsoft 365 for business ו-Office עבור Mac.

- השתמש [בכלי הפריסה של office](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) כדי לא לכלול צוותים מהתקנות חדשות של Office.
- כדי *להסיר את התקנת* teams ממכשיר שבו פועל Windows, ראה [הסרת ההתקנה של Microsoft teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). כדי לנקות את Microsoft Teams ממחשבי יעד או ממשתמשים מרובים, ראה [ניקוי הפריסה של Microsoft teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).
- השתמש באפשרות [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) כדי למנוע מ-Microsoft teams להתקין באופן אוטומטי עם Office.
- השתמש באפשרות [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) , *לפני התקנת teams*, כדי למנוע הפעלה אוטומטית של Microsoft teams לאחר ההתקנה.

אם אתה משתמש ב-Office עבור Mac, ראה [התקנות Microsoft teams ב-mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).