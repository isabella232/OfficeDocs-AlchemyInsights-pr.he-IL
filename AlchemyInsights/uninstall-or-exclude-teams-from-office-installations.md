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
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="2649f-102">הסרת התקנה או אי-הכללה של Teams מהתקנות חדשות או קיימות של Office</span><span class="sxs-lookup"><span data-stu-id="2649f-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="2649f-103">Microsoft Teams כלול כחלק מ-Microsoft 365 Apps עבור enterprise, יישומי Microsoft 365 for business ו-Office עבור Mac.</span><span class="sxs-lookup"><span data-stu-id="2649f-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="2649f-104">השתמש [בכלי הפריסה של office](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) כדי לא לכלול צוותים מהתקנות חדשות של Office.</span><span class="sxs-lookup"><span data-stu-id="2649f-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="2649f-105">כדי *להסיר את התקנת* teams ממכשיר שבו פועל Windows, ראה [הסרת ההתקנה של Microsoft teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span><span class="sxs-lookup"><span data-stu-id="2649f-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="2649f-106">כדי לנקות את Microsoft Teams ממחשבי יעד או ממשתמשים מרובים, ראה [ניקוי הפריסה של Microsoft teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span><span class="sxs-lookup"><span data-stu-id="2649f-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="2649f-107">השתמש באפשרות [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) כדי למנוע מ-Microsoft teams להתקין באופן אוטומטי עם Office.</span><span class="sxs-lookup"><span data-stu-id="2649f-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="2649f-108">השתמש באפשרות [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) , *לפני התקנת teams*, כדי למנוע הפעלה אוטומטית של Microsoft teams לאחר ההתקנה.</span><span class="sxs-lookup"><span data-stu-id="2649f-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="2649f-109">אם אתה משתמש ב-Office עבור Mac, ראה [התקנות Microsoft teams ב-mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span><span class="sxs-lookup"><span data-stu-id="2649f-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>