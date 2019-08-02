---
title: פריסת צוותים כקובץ עצמאי או עם התקנות Office חדש או קיים
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 08/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 3318e1b17cc99e927e1011f7ca9eca8dec616d59
ms.sourcegitcommit: 4600dd4fb577bf5f5482a24616c2d9a6b81e8052
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/01/2019
ms.locfileid: "36054232"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>פריסת צוותים כקובץ עצמאי או עם התקנות Office חדש או קיים

צוותים Microsoft היא כעת כלולים כחלק ***התקנות חדשות*** של Office 365 ProPlus, Office 365 עסקיים ו- Office for mac לקבלת מידע נוסף, ראה [כאשר צוותים Microsoft תתחיל הכלולה התקנות חדשות של Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)

בנוסף, החל ב- 1906 גירסה בערוץ חודשי, צוותים יהיה ***להוסיף התקנות קיימות*** של Office 365 ProPlus (ואביזרי Office 365) במכשירים פועל בעת עדכון ההתקנה הקיימת שלך לגירסה העדכנית ביותר של Windows. לקבלת מידע נוסף, ראה [מה לגבי התקנות קיימות של Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)

> [!NOTE]
> אם אין ברצונך להמתין לוח זמנים זה ההשקה, באפשרותך לפרוס צוותים כקובץ עצמאי עבור המשתמשים שלך על-ידי [ביצוע הוראות אלה](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) או לאפשר למשתמשים להתקין צוותים עבור עצמם מתוך [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).

אם הארגון שלך אינו מוכן לפרוס צוותים, יש לנו את השלבים שבאפשרותך לבצע כדי ***לא לכלול צוותים*** מהתקנות [חדש](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) או [קיים](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) של Office. אם ברצונך לצוותים להיות מותקן, אך אינך מעוניין צוותים להתחיל באופן אוטומטי עבור המשתמש לאחר התקנתו, ראה [צוותים Microsoft מונעת ממנו לפעול באופן אוטומטי לאחר ההתקנה](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

כדי ***להסיר את ההתקנה של צוותים*** מתוך התקן שפועל בו Windows, ראה [הסרת התקנה צוותים Microsoft](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). ניקוי לצוותים Microsoft במחשבי יעד מרובים או משתמשים, ראה [פריסת Microsoft צוותים לנקות](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

אם אתה משתמש מחשבים משותפים, שירותי שולחן עבודה מרוחק (RDS) או תשתית שולחן עבודה וירטואלי (VDI), ראה [מחשב משותף ובסביבות VDI עם צוותים של Microsoft](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

אם אתה משתמש ב- Office for Mac, ראה [התקנות צוותים Microsoft ב- Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> לאחר התקנת צוותים, הוא [מתעדכן אוטומטית](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) משבועיים עם תכונות חדשות ועדכונים איכות. 