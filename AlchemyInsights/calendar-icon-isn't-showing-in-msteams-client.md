---
title: סמל לוח השנה אינו מוצג בלקוח Microsoft Teams
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583532"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a><span data-ttu-id="5e97e-102">סמל לוח השנה אינו מוצג בלקוח Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="5e97e-102">Calendar icon isn't showing in Microsoft Teams client</span></span>

<span data-ttu-id="5e97e-103">הכרטיסיה ' **לוח שנה** ' ב-teams מחייבת גישה לתיבת דואר של exchange באמצעות Exchange Web Services.</span><span class="sxs-lookup"><span data-stu-id="5e97e-103">The **Calendar** Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="5e97e-104">תיבת הדואר של Exchange יכולה להיות מקוונת או מקומית.</span><span class="sxs-lookup"><span data-stu-id="5e97e-104">The Exchange mailbox can be Online, or On-Premises.</span></span> <span data-ttu-id="5e97e-105">עבור משתמשים מקוונים שאינם רואים את הכרטיסיה **לוח שנה** , ודא שהוא [מורשה עבור תיבת דואר של Exchange Online ושתיבת הדואר מאופשרת](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="5e97e-105">For Online users who do not see the **Calendar** Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span> <span data-ttu-id="5e97e-106">אם המשתמשים שלך מוצגים באופן מקומי, עליך לוודא שהתצורה ההיברידית שלך בריאה.</span><span class="sxs-lookup"><span data-stu-id="5e97e-106">If your users are homed On-Premises, you need to confirm that your Hybrid configuration is healthy.</span></span> <span data-ttu-id="5e97e-107">השתמש ב- [אשף קביעת התצורה ההיברידית](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) כדי לפתור בעיות.</span><span class="sxs-lookup"><span data-stu-id="5e97e-107">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span> <span data-ttu-id="5e97e-108">שים לב כי [Teams דורש גירסת Exchange 2016 CU3 או גבוהה יותר](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="5e97e-108">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>

<span data-ttu-id="5e97e-109">לקבלת מידע נוסף ושלבי פתרון בעיות, ראה [פתרון בעיות של Microsoft teams ואינטראקציה של Exchange Server](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span><span class="sxs-lookup"><span data-stu-id="5e97e-109">For more information and troubleshooting steps, see [Troubleshoot Microsoft Teams and Exchange Server interaction issues](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span></span>
