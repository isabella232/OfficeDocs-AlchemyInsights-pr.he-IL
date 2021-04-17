---
title: הסרת התקנה או אי-הכללה של Teams מהתקנות Office
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
ms.openlocfilehash: 2d96d54cb479f5f52cc707d4307cf9cf1e891a01
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827793"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="f29c7-102">הסרת התקנה או אי-הכללה של Teams מהתקנות חדשות או קיימות של Office</span><span class="sxs-lookup"><span data-stu-id="f29c7-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="f29c7-103">Microsoft Teams כלול כחלק מאפליקציות Microsoft 365 עבור הארגון, יישומי Microsoft 365 לעסקים ו- Office for Mac.</span><span class="sxs-lookup"><span data-stu-id="f29c7-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="f29c7-104">השתמש בכלי [הפריסה של Office כדי](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) לא לכלול את Teams בהתקנות חדשות של Office.</span><span class="sxs-lookup"><span data-stu-id="f29c7-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="f29c7-105">כדי *להסיר את ההתקנה* של Teams ממכשיר שבו פועל Windows, ראה [הסרת ההתקנה של Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span><span class="sxs-lookup"><span data-stu-id="f29c7-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="f29c7-106">כדי לנקות את Microsoft Teams ממחשבים או משתמשים מרובים של יעד, ראה [ניקוי פריסת Microsoft Teams](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span><span class="sxs-lookup"><span data-stu-id="f29c7-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="f29c7-107">השתמש באפשרות [PreventTeamsInstall כדי](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) למנוע התקנה אוטומטית של Microsoft Teams באמצעות Office.</span><span class="sxs-lookup"><span data-stu-id="f29c7-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="f29c7-108">השתמש באפשרות [PreventFirstLaunchAfterInstall,](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) *לפני התקנת Teams*, כדי למנוע הפעלה אוטומטית של Microsoft Teams לאחר ההתקנה.</span><span class="sxs-lookup"><span data-stu-id="f29c7-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="f29c7-109">אם אתה משתמש ב- Office עבור Mac, ראה [התקנות Microsoft Teams ב- Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span><span class="sxs-lookup"><span data-stu-id="f29c7-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>