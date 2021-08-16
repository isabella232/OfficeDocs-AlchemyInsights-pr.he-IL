---
title: פריסת Teams עצמאית או עם התקנות חדשות או Office קיימות
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: e8baefafc1c2f9583345779c5ae7a9d3d0e05c4b3b7e1b3a74a9a22f7ceed02a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102203"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>פריסת Teams עצמאית או עם התקנות חדשות או Office קיימות

Microsoft Teams נכלל כעת כחלק מהתקנות ***חדשות*** של יישומי Microsoft 365 לארגונים, יישומי Microsoft 365 לעסקים ו- Office עבור Mac. לקבלת מידע נוסף, [ראה מתי Microsoft Teams להיכלל בהתקנות חדשות של Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

בנוסף, החל מגירסה 1906 בערוץ הנוכחי, Teams  יתווסף להתקנות קיימות של יישומי Microsoft 365 לארגונים (ו- יישומי Microsoft 365 לעסקים) במכשירים פועלים Windows בעת עדכון ההתקנה הקיימת לגירסה העדכנית ביותר. לקבלת מידע נוסף, [ראה מה לגבי התקנות קיימות של Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> אם אינך מעוניין להמתין ללוח זמנים זה של ההפרשה, באפשרותך לפרוס את Teams כעצמן עבור המשתמשים שלך על-ידי ביצוע הוראות [אלה](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) או לאפשר למשתמשים שלך להתקין Teams עבור עצמם [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) מ- .

אם הארגון שלך אינו מוכן לפרוס Teams, יש לנו את השלבים ש באפשרותך [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) לבצע [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) ***כדי לא לכלול Teams*** התקנות חדשות או קיימות של Office. אם ברצונך Teams, אך אינך מעוניין ש- Teams יופעל באופן אוטומטי עבור המשתמש לאחר התקנתו, ראה מניעת [הפעלה אוטומטית של Microsoft Teams לאחר ההתקנה.](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)

כדי ***להסיר Teams התקנה*** ממכשיר שבו פועל Windows, ראה הסרת [Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). כדי לנקות Microsoft Teams מחשבים או משתמשים מרובים של יעד, [ראה ניקוי Microsoft Teams פריסה.](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

אם אתה משתמש במחשבים משותפים, שירותי שולחן עבודה מרוחק (RDS) או תשתית שולחן עבודה וירטואלי (VDI), ראה מחשבים משותפים וסביבות [VDI עם Microsoft Teams.](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)

אם אתה משתמש ב- Office עבור Mac, [ראה Microsoft Teams התקנות ב- Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> לאחר Teams מותקן, הוא מתעדכן [באופן](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) אוטומטי כל שבועיים עם תכונות חדשות ועדכונים איכותיים. 