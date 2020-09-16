---
title: צוותים מותקנים באמצעות עדכוני Office
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
- "2599"
- "9000140"
- "9000660"
- "2509"
ms.openlocfilehash: 9a09800fcc36876629c7d59182f20b5b16393ef8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47736505"
---
# <a name="microsoft-teams-installed-with-office-updates"></a>Microsoft Teams מותקנים באמצעות עדכוני Office

Microsoft Teams כלול כחלק ***מהתקנות חדשות*** של יישומי microsoft 365 עבור Enterprise, יישומי microsoft 365 for business ו-Office עבור Mac. לקבלת מידע נוסף, ראה [מתי Microsoft teams יתחיל להיכלל בהתקנות חדשות של Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

בנוסף, החל מגירסה 1906 בערוץ הנוכחי, הצוותים יתווספו בהדרגה ***להתקנות קיימות*** של יישומי Microsoft 365 עבור enterprise (ו-Microsoft 365 apps לעסקים) במכשירים שבהם פועל Windows בעת עדכון ההתקנה הקיימת לגירסה העדכנית ביותר. לקבלת מידע נוסף, ראה [מה לגבי התקנות קיימות של Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**הערה:** אם אינך מעוניין להמתין ללוח הזמנים של ההשקה, באפשרותך לפרוס את Teams כעצמאיים עבור המשתמשים שלך על-ידי [ביצוע הוראות אלה](https://docs.microsoft.com/MicrosoftTeams/msi-deployment), או לאפשר למשתמשים שלך להתקין את teams עבור עצמם https://teams.microsoft.com/downloads .

אם הארגון שלך אינו מוכן לפרוס את Teams, באפשרותך ***לכלול את teams*** מהתקנות [חדשות](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) או [קיימות](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) של Office. אם ברצונך להתקין את Teams, אך אינך מעוניין ש-Teams יופעלו באופן אוטומטי עבור המשתמש לאחר התקנתו, ראה [מנע מ-Microsoft teams לפעול באופן אוטומטי לאחר ההתקנה](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

כדי ***להסיר את התקנת teams*** ממכשיר שבו פועל Windows, ראה [הסרת ההתקנה של Microsoft teams](https://support.office.com/article/uninstall-microsoft-teams-3b159754-3c26-4952-abe7-57d27f5f4c81). כדי לנקות את Microsoft Teams ממחשבי יעד או ממשתמשים מרובים, ראה [ניקוי הפריסה של Microsoft teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

אם אתה משתמש במחשבים משותפים, בשירותי שולחן עבודה מרוחק (RDS) או בתשתית שולחן עבודה וירטואלי (VDI), ראה [סביבות מחשב משותפות וVDI עם Microsoft teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams). אם אתה משתמש ב-Office עבור Mac, ראה [התקנות Microsoft teams ב-mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

**הערה:** לאחר התקנת Teams, היא [מתעדכנת באופן אוטומטי](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) בערך כל שבועיים באמצעות תכונות חדשות ועדכונים איכותיים. 