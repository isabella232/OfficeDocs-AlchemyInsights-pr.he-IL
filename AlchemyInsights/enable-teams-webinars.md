---
title: הפיכת Teams Webinars לזמינים
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793648"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="a8246-102">הפיכת Teams Webinars לזמינים</span><span class="sxs-lookup"><span data-stu-id="a8246-102">Enable Teams Webinars</span></span>

<span data-ttu-id="a8246-103">Webinars זמינים כברירת מחדל.</span><span class="sxs-lookup"><span data-stu-id="a8246-103">Webinars are enabled by default.</span></span> <span data-ttu-id="a8246-104">באפשרותך לנהל מי יכול לתזמן ולרשום Teams Webinars באמצעות Teams PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a8246-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="a8246-105">כל המשתמשים שיכולים ליצור פגישה יכולים גם ליצור פגישת סמינר מקוון.</span><span class="sxs-lookup"><span data-stu-id="a8246-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="a8246-106">אם ברצונך לנהל מי יכול לתזמן Teams אינטרנט, השתמש *ב- AllowMeetingRegistration*.</span><span class="sxs-lookup"><span data-stu-id="a8246-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="a8246-107">כברירת מחדל, *WhoCanRegister* זמין ומגדיר **את** כולם.</span><span class="sxs-lookup"><span data-stu-id="a8246-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="a8246-108">אם ברצונך לבטל את רישום הפגישה, הגדר *את AllowMeetingRegistration ל-* **False**.</span><span class="sxs-lookup"><span data-stu-id="a8246-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="a8246-109">כדי לשנות הגדרות אלה, עליך להתקין [את Teams PowerShell](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="a8246-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="a8246-110">כמו כן, מדיניות פגישה נאכפת על-ידי Teams Webinars.</span><span class="sxs-lookup"><span data-stu-id="a8246-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="a8246-111">לדוגמה, אם ההצטרפות האנונימית מבוטלת בהגדרות הפגישה, משתמשים אנונימיים לא יכולים להצטרף ל- webinars.</span><span class="sxs-lookup"><span data-stu-id="a8246-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="a8246-112">לקבלת מידע נוסף על קביעת התצורה של מי יכול להירשם לאתרי אינטרנט, ראה [קביעת תצורה של מי יכול להירשם עבור webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span><span class="sxs-lookup"><span data-stu-id="a8246-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="a8246-113">לקבלת מידע נוסף אודות הגדרות עבור רשימות Microsoft, ראה [הגדרות שליטה עבור רשימות Microsoft.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="a8246-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>