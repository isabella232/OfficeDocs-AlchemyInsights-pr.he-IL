---
title: ניהול רישום סמינר מקוון
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793917"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="d9882-102">ניהול רישום סמינר מקוון</span><span class="sxs-lookup"><span data-stu-id="d9882-102">Manage webinar registration</span></span>

<span data-ttu-id="d9882-103">באפשרותך לנהל מי יכול להירשם Teams Webinars באמצעות Teams Powershell.</span><span class="sxs-lookup"><span data-stu-id="d9882-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="d9882-104">כדי להתקין Teams Powershell, ראה [Teams PowerShell](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="d9882-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="d9882-105">כברירת מחדל, *WhoCanRegister* זמין ומוגדר **ל- EveryoneInCompany**.</span><span class="sxs-lookup"><span data-stu-id="d9882-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="d9882-106">כדי לאפשר לכל אדם, כולל משתמשים אנונימיים, להירשם, עליך להגדיר את מדיניות **הפגישה** לכולם באמצעות הפקודה Powershell:</span><span class="sxs-lookup"><span data-stu-id="d9882-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="d9882-107">**הערה**: אם ההצטרפות האנונימית מבוטלת בהגדרות הפגישה, משתמשים אנונימיים לא יכולים להצטרף ל- webinars.</span><span class="sxs-lookup"><span data-stu-id="d9882-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="d9882-108">כדי ללמוד עוד ולאפשר הגדרה זו, ראה [ניהול הגדרות פגישה ב- Microsoft Teams.](/microsoftteams/meeting-settings-in-teams)</span><span class="sxs-lookup"><span data-stu-id="d9882-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="d9882-109">אם ברצונך לבטל את רישום הפגישה, הגדר *את AllowMeetingRegistration ל-* **False**.</span><span class="sxs-lookup"><span data-stu-id="d9882-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="d9882-110">לקבלת מידע נוסף על קביעת התצורה של מי יכול להירשם לאתרי אינטרנט, ראה [קביעת תצורה של מי יכול להירשם עבור webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="d9882-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="d9882-111">לקבלת מידע נוסף אודות הגדרות עבור רשימות Microsoft, ראה [הגדרות שליטה עבור רשימות Microsoft.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="d9882-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
