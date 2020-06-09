---
title: צוותים המותקנים באמצעות עדכוני Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2599"
- "9000140"
- "9000660"
- "2509"
ms.openlocfilehash: 34593fbe80f11c9b4e1d10d3e1dbe5ff79602299
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/09/2020
ms.locfileid: "44617965"
---
# <a name="microsoft-teams-installed-with-office-updates"></a>צוותי Microsoft המותקנים עם עדכוני Office

צוותי microsoft נכללים כחלק ***מהתקנות חדשות*** של Microsoft 365 apps עבור הארגון, Microsoft 365 apps לעסקים ו-Office for Mac. לקבלת מידע נוסף, ראה מתי הנתונים של [Microsoft יתחילו להיכלל בהתקנות חדשות של Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

בנוסף, החל בגירסה 1906 בערוץ הנוכחי, הצוותים יתווספו בהדרגה ***להתקנות קיימות*** של Microsoft 365 Apps עבור הארגון (ו-Microsoft 365 apps לעסקים) בהתקנים המפעילים את Windows בעת עדכון ההתקנה הקיימת לגירסה העדכנית. לקבלת מידע נוסף, ראה [מה לגבי התקנות קיימות של Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**הערה:** אם אין ברצונך להמתין ללוח הזמנים של ההשקה, באפשרותך לפרוס צוותים כעצמאיים עבור המשתמשים שלך על-ידי [ביצוע הוראות אלה](https://docs.microsoft.com/MicrosoftTeams/msi-deployment), או לאפשר למשתמשים שלך להתקין צוותים מעצמם https://teams.microsoft.com/downloads .

אם הארגון שלך אינו מוכן לפרוס צוותים, באפשרותך לא ***לכלול צוותים*** מהתקנות [חדשות](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) או [קיימות](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) של Office. אם ברצונך להתקין את הצוותים, אך אין ברצונך שהקבוצות יתחילו באופן אוטומטי עבור המשתמש לאחר התקנתה, ראה [מניעת הפעלה אוטומטית של צוותי Microsoft לאחר ההתקנה](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

כדי ***להסיר את ההתקנה של צוותים*** מהתקן שבו פועל Windows, ראה [הסרת התקנה של צוותי Microsoft](https://support.office.com/article/uninstall-microsoft-teams-3b159754-3c26-4952-abe7-57d27f5f4c81). כדי לנקות צוותים של Microsoft ממחשבי יעד או משתמשים מרובים, ראה [ניקוי הפריסה של צוותי microsoft](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

אם אתה משתמש במחשבים משותפים, בשירותי שולחן עבודה מרוחק (RDS) או בתשתית שולחן עבודה וירטואלי (VDI), ראה [סביבת מחשב משותפת וסביבות vdi עם צוותי Microsoft](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams). אם אתה משתמש ב-Office for Mac, ראה [התקנות Microsoft נבחרות ב-Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

**הערה:** לאחר התקנת הצוותים, הוא [מתעדכן באופן אוטומטי](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) כ-2 שבועות עם תכונות חדשות ועדכונים איכותיים. 