---
title: פריסת צוותים כעצמאיים או עם התקנות Office חדשות או קיימות
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 5ec5277a758fc5171c846266787c2fbcf751f21c
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/09/2020
ms.locfileid: "44617896"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>פריסת צוותים כעצמאיים או עם התקנות Office חדשות או קיימות

צוותי microsoft כלולים כעת כחלק ***מהתקנות חדשות*** של Microsoft 365 apps עבור הארגון, Microsoft 365 apps עבור עסקים ו-Office for Mac. לקבלת מידע נוסף, ראה מתי הנתונים של [Microsoft יתחילו להיכלל בהתקנות חדשות של Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

בנוסף, החל בגירסה 1906 בערוץ הנוכחי, הצוותים ***יתווספו להתקנות הקיימות*** של Microsoft 365 Apps עבור הארגון (ו-Microsoft 365 apps לעסקים) בהתקנים המפעילים את Windows כאשר תעדכן את ההתקנה הקיימת שלך בגירסה העדכנית ביותר. לקבלת מידע נוסף, ראה [מה לגבי התקנות קיימות של Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> אם אין ברצונך להמתין ללוח הזמנים של ההשקה, באפשרותך לפרוס צוותים כעצמאיים עבור המשתמשים שלך על-ידי [ביצוע הוראות אלה](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)   או שאתה יכול לבקש מהמשתמשים להתקין צוותים מעצמם https://teams.microsoft.com/downloads .

אם הארגון שלך אינו מוכן לפרוס צוותים, יש לנו את הצעדים שבאפשרותך לנקוט כדי לא ***לכלול צוותים*** מהתקנות [חדשות](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) או [קיימות](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) של Office. אם ברצונך להתקין את הצוותים, אך אין ברצונך שהקבוצות יתחילו באופן אוטומטי עבור המשתמש לאחר התקנתה, ראה [מניעת הפעלה אוטומטית של צוותי Microsoft לאחר ההתקנה](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

כדי ***להסיר את ההתקנה של צוותים*** מהתקן שבו פועל Windows, ראה [הסרת התקנה של צוותי Microsoft](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). כדי לנקות את צוותי Microsoft ממחשבי יעד או משתמשים מרובים, ראה [הפריסה של צוותי microsoft נקיה](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

אם אתה משתמש במחשבים משותפים, בשירותי שולחן עבודה מרוחק (RDS) או בתשתית שולחן עבודה וירטואלי (VDI), ראה [סביבת מחשב משותפת וסביבות vdi עם צוותי Microsoft](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

אם אתה משתמש ב-Office for Mac, ראה [התקנות Microsoft נבחרות ב-Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> לאחר התקנת הצוותים, הוא [מתעדכן באופן אוטומטי](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) כ-2 שבועות עם תכונות חדשות ועדכונים איכותיים. 