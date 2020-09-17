---
title: פריסת צוותים כעצמאיים או באמצעות התקנות Office חדשות או קיימות
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
ms.openlocfilehash: c3ca4365abc41509ccf602c5b9046655706840fc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806760"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a><span data-ttu-id="411c6-102">פריסת צוותים כעצמאיים או באמצעות התקנות Office חדשות או קיימות</span><span class="sxs-lookup"><span data-stu-id="411c6-102">Deploying Teams as standalone or with new or existing Office installations</span></span>

<span data-ttu-id="411c6-103">Microsoft Teams כלול כעת כחלק ***מהתקנות חדשות*** של יישומי microsoft 365 עבור Enterprise, יישומי microsoft 365 for business ו-Office עבור Mac.</span><span class="sxs-lookup"><span data-stu-id="411c6-103">Microsoft Teams is now included as part of ***new installations*** of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span> <span data-ttu-id="411c6-104">לקבלת מידע נוסף, ראה [מתי Microsoft teams יתחיל להיכלל בהתקנות חדשות של Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)</span><span class="sxs-lookup"><span data-stu-id="411c6-104">For more information, see [When will Microsoft Teams start being included with new installations of Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)</span></span>

<span data-ttu-id="411c6-105">בנוסף, החל מגירסה 1906 בערוץ הנוכחי, Teams ***יתווספו להתקנות קיימות*** של יישומי Microsoft 365 עבור enterprise (ו-microsoft 365 לעסקים) במכשירים שבהם פועל Windows בעת עדכון ההתקנה הקיימת לגירסה העדכנית ביותר.</span><span class="sxs-lookup"><span data-stu-id="411c6-105">Additionally, starting with Version 1906 in Current Channel , Teams will be ***added to existing installations*** of Microsoft 365 Apps for enterprise (and Microsoft 365 Apps for business) on devices running Windows when you update your existing installation to the latest version.</span></span> <span data-ttu-id="411c6-106">לקבלת מידע נוסף, ראה [מה לגבי התקנות קיימות של Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)</span><span class="sxs-lookup"><span data-stu-id="411c6-106">For more information, see [What about existing installations of Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)</span></span>

> [!NOTE]
> <span data-ttu-id="411c6-107">אם אינך מעוניין להמתין ללוח הזמנים של ההשקה, באפשרותך לפרוס את Teams כעצמאיים עבור המשתמשים שלך על-ידי [ביצוע הוראות אלה](https://docs.microsoft.com/MicrosoftTeams/msi-deployment),   או לאפשר למשתמשים שלך להתקין את teams עבור עצמם  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .</span><span class="sxs-lookup"><span data-stu-id="411c6-107">If you don't want to wait for this rollout schedule, you can deploy Teams as standalone for your users by [following these instructions](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) or you can have your users install Teams for themselves from [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads).</span></span>

<span data-ttu-id="411c6-108">אם הארגון שלך אינו מוכן לפרוס את Teams, יש לנו את השלבים שניתן לבצע כדי לא ***לכלול את teams*** מהתקנות [חדשות](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) או [קיימות](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) של Office.</span><span class="sxs-lookup"><span data-stu-id="411c6-108">If your organization isn't ready to deploy Teams, we have the steps you can take to ***exclude Teams*** from [new](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) or [existing](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) installations of Office.</span></span> <span data-ttu-id="411c6-109">אם ברצונך להתקין את Teams, אך אינך מעוניין ש-Teams יופעלו באופן אוטומטי עבור המשתמש לאחר התקנתו, ראה [מנע מ-Microsoft teams לפעול באופן אוטומטי לאחר ההתקנה](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).</span><span class="sxs-lookup"><span data-stu-id="411c6-109">If you want Teams to be installed, but don't want Teams to start automatically for the user after it's installed, see [Prevent Microsoft Teams from starting automatically after installation](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).</span></span>

<span data-ttu-id="411c6-110">כדי ***להסיר את התקנת teams*** ממכשיר שבו פועל Windows, ראה [הסרת ההתקנה של Microsoft teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span><span class="sxs-lookup"><span data-stu-id="411c6-110">To ***uninstall Teams*** from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="411c6-111">כדי לנקות את Microsoft Teams ממחשבי יעד או ממשתמשים מרובים, ראה [ניקוי הפריסה של Microsoft teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span><span class="sxs-lookup"><span data-stu-id="411c6-111">To cleanup Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>

<span data-ttu-id="411c6-112">אם אתה משתמש במחשבים משותפים, בשירותי שולחן עבודה מרוחק (RDS) או בתשתית שולחן עבודה וירטואלי (VDI), ראה [סביבות מחשב משותפות וVDI עם Microsoft teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).</span><span class="sxs-lookup"><span data-stu-id="411c6-112">If you're using shared computers, Remote Desktop Services (RDS), or Virtual Desktop Infrastructure (VDI), see [Shared computer and VDI environments with Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).</span></span>

<span data-ttu-id="411c6-113">אם אתה משתמש ב-Office עבור Mac, ראה [התקנות Microsoft teams ב-mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span><span class="sxs-lookup"><span data-stu-id="411c6-113">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>

> [!NOTE]
> <span data-ttu-id="411c6-114">לאחר התקנת Teams, היא [מתעדכנת באופן אוטומטי](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) בערך כל שבועיים באמצעות תכונות חדשות ועדכונים איכותיים.</span><span class="sxs-lookup"><span data-stu-id="411c6-114">After Teams is installed, it's [automatically updated](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) approximately every two weeks with new features and quality updates.</span></span> 