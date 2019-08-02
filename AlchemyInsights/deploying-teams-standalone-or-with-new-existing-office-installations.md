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
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a><span data-ttu-id="df819-102">פריסת צוותים כקובץ עצמאי או עם התקנות Office חדש או קיים</span><span class="sxs-lookup"><span data-stu-id="df819-102">Deploying Teams as standalone or with new or existing Office installations</span></span>

<span data-ttu-id="df819-103">צוותים Microsoft היא כעת כלולים כחלק ***התקנות חדשות*** של Office 365 ProPlus, Office 365 עסקיים ו- Office for mac</span><span class="sxs-lookup"><span data-stu-id="df819-103">Microsoft Teams is now included as part of ***new installations*** of Office 365 ProPlus, Office 365 Business, and Office for Mac.</span></span> <span data-ttu-id="df819-104">לקבלת מידע נוסף, ראה [כאשר צוותים Microsoft תתחיל הכלולה התקנות חדשות של Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)</span><span class="sxs-lookup"><span data-stu-id="df819-104">For more information, see [When will Microsoft Teams start being included with new installations of Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-office-365-proplus)</span></span>

<span data-ttu-id="df819-105">בנוסף, החל ב- 1906 גירסה בערוץ חודשי, צוותים יהיה ***להוסיף התקנות קיימות*** של Office 365 ProPlus (ואביזרי Office 365) במכשירים פועל בעת עדכון ההתקנה הקיימת שלך לגירסה העדכנית ביותר של Windows.</span><span class="sxs-lookup"><span data-stu-id="df819-105">Additionally, starting with Version 1906 in Monthly Channel, Teams will be ***added to existing installations*** of Office 365 ProPlus (and Office 365 Business) on devices running Windows when you update your existing installation to the latest version.</span></span> <span data-ttu-id="df819-106">לקבלת מידע נוסף, ראה [מה לגבי התקנות קיימות של Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)</span><span class="sxs-lookup"><span data-stu-id="df819-106">For more information, see [What about existing installations of Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-office-365-proplus)</span></span>

> [!NOTE]
> <span data-ttu-id="df819-107">אם אין ברצונך להמתין לוח זמנים זה ההשקה, באפשרותך לפרוס צוותים כקובץ עצמאי עבור המשתמשים שלך על-ידי [ביצוע הוראות אלה](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) או לאפשר למשתמשים להתקין צוותים עבור עצמם מתוך [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).</span><span class="sxs-lookup"><span data-stu-id="df819-107">If you don't want to wait for this rollout schedule, you can deploy Teams as standalone for your users by [following these instructions](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) or you can have your users install Teams for themselves from [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).</span></span>

<span data-ttu-id="df819-108">אם הארגון שלך אינו מוכן לפרוס צוותים, יש לנו את השלבים שבאפשרותך לבצע כדי ***לא לכלול צוותים*** מהתקנות [חדש](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) או [קיים](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) של Office.</span><span class="sxs-lookup"><span data-stu-id="df819-108">If your organization isn't ready to deploy Teams, we have the steps you can take to ***exclude Teams*** from [new](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-office-365-proplus) or [existing](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) installations of Office.</span></span> <span data-ttu-id="df819-109">אם ברצונך לצוותים להיות מותקן, אך אינך מעוניין צוותים להתחיל באופן אוטומטי עבור המשתמש לאחר התקנתו, ראה [צוותים Microsoft מונעת ממנו לפעול באופן אוטומטי לאחר ההתקנה](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).</span><span class="sxs-lookup"><span data-stu-id="df819-109">If you want Teams to be installed, but don't want Teams to start automatically for the user after it's installed, see [Prevent Microsoft Teams from starting automatically after installation](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).</span></span>

<span data-ttu-id="df819-110">כדי ***להסיר את ההתקנה של צוותים*** מתוך התקן שפועל בו Windows, ראה [הסרת התקנה צוותים Microsoft](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span><span class="sxs-lookup"><span data-stu-id="df819-110">To ***uninstall Teams*** from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="df819-111">ניקוי לצוותים Microsoft במחשבי יעד מרובים או משתמשים, ראה [פריסת Microsoft צוותים לנקות](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span><span class="sxs-lookup"><span data-stu-id="df819-111">To cleanup Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>

<span data-ttu-id="df819-112">אם אתה משתמש מחשבים משותפים, שירותי שולחן עבודה מרוחק (RDS) או תשתית שולחן עבודה וירטואלי (VDI), ראה [מחשב משותף ובסביבות VDI עם צוותים של Microsoft](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).</span><span class="sxs-lookup"><span data-stu-id="df819-112">If you're using shared computers, Remote Desktop Services (RDS), or Virtual Desktop Infrastructure (VDI), see [Shared computer and VDI environments with Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).</span></span>

<span data-ttu-id="df819-113">אם אתה משתמש ב- Office for Mac, ראה [התקנות צוותים Microsoft ב- Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span><span class="sxs-lookup"><span data-stu-id="df819-113">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>

> [!NOTE]
> <span data-ttu-id="df819-114">לאחר התקנת צוותים, הוא [מתעדכן אוטומטית](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) משבועיים עם תכונות חדשות ועדכונים איכות.</span><span class="sxs-lookup"><span data-stu-id="df819-114">After Teams is installed, it's [automatically updated](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) approximately every two weeks with new features and quality updates.</span></span> 