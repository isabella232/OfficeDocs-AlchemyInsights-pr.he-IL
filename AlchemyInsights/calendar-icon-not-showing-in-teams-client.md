---
title: סמל לוח שנה אינו מופיע אצל לקוח Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932207"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="60969-102">סמל לוח שנה אינו מופיע אצל לקוח Teams</span><span class="sxs-lookup"><span data-stu-id="60969-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="60969-103">הכרטיסייה 'לוח שנה' ב-Teams מחייבת גישה לתיבת דואר של Exchange דרך Exchange Web Services.</span><span class="sxs-lookup"><span data-stu-id="60969-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="60969-104">תיבת הדואר של Exchange יכול להיות מקוונת או מקומית.</span><span class="sxs-lookup"><span data-stu-id="60969-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="60969-105">עבור משתמשים מקוונים שאין רואים את הכרטיסייה ‘לוח שנה‘, ודא שהם [בעלי רישיון לתיבת דואר של Exchange Online ושתיבת הדואר זמינה](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="60969-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="60969-106">אם למשתמש יש תיבת דואר חוקית ב- Exchange Online, אבל הוא עדיין לא יכול לראות את הכרטיסייה ‘לוח שנה‘, ייתכן שאתה נתקל בבעיית רשת.</span><span class="sxs-lookup"><span data-stu-id="60969-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="60969-107">השתמש ב- [מנח הקישוריות המרוחקת של Microsoft](https://testconnectivity.microsoft.com/) והפעל את **בדיקות הקישוריות של שירותי האינטרנט של Microsoft Exchange**עבוד המשתמש המושפע.</span><span class="sxs-lookup"><span data-stu-id="60969-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="60969-108">לסיום, בדוק את [אפליקציות של Teams - מדיניות הגדרת אפליקציה](https://admin.teams.microsoft.com/policies/app-setup) כדי לוודא שיישום לוח השנה לא הוסר מהמדיניות שחלה על המשתמש (סביר להניח ש **(ברירת המחדל ברחבי הארגון) הכללית**.</span><span class="sxs-lookup"><span data-stu-id="60969-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="60969-109">אם המשתמשים שלך ממוקמים בבית, עליך לאשר כי קביעת התצורה ההיברידית שלך תקינה.</span><span class="sxs-lookup"><span data-stu-id="60969-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="60969-110">השתמש ב- [אשף קביעת התצורה ההיברידית](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) כדי לפתור בעיות.</span><span class="sxs-lookup"><span data-stu-id="60969-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="60969-111">שים לב כי [Teams דורש גירסת Exchange 2016 CU3 או גבוהה יותר](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="60969-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
