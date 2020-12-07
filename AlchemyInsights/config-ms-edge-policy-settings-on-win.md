---
title: קביעת התצורה של הגדרות מדיניות הקצה של Microsoft ב-Windows
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
- "9003845"
- "6894"
ms.openlocfilehash: 7f626152c3833638436dfe05e8dcd13fc86ef594
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583442"
---
# <a name="configure-microsoft-edge-policy-settings-on-windows"></a><span data-ttu-id="a3e7b-102">קביעת התצורה של הגדרות מדיניות הקצה של Microsoft ב-Windows</span><span class="sxs-lookup"><span data-stu-id="a3e7b-102">Configure Microsoft Edge policy settings on Windows</span></span>

<span data-ttu-id="a3e7b-103">כדי לקבוע תצורה של הגדרות מדיניות ועדכונים מנוהלים עבור Microsoft Edge, השתמש באובייקטי מדיניות קבוצתית (Gpo).</span><span class="sxs-lookup"><span data-stu-id="a3e7b-103">To configure policy settings and managed updates for Microsoft Edge, use Group Policy Objects (GPOs).</span></span> <span data-ttu-id="a3e7b-104">באפשרותך גם להקצות מדיניות באמצעות הרישום; אפשרות זו מתאימה (1) מכשירים של Windows המחוברים לתחום של Microsoft Active Directory ולמופעים (2) של Windows 10 Pro ו-Enterprise שנרשמו לניהול מכשירים ב-Microsoft intune.</span><span class="sxs-lookup"><span data-stu-id="a3e7b-104">You can also provision policy through the registry; this would be appropriate for (1) Windows devices joined to a Microsoft Active Directory domain and for (2) Windows 10 Pro and Enterprise instances enrolled for device management in Microsoft Intune.</span></span>

<span data-ttu-id="a3e7b-105">כדי לקבוע את התצורה של Microsoft Edge באמצעות אובייקטי Gpo, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="a3e7b-105">To configure Microsoft Edge by using GPOs, do the following:</span></span>

1. <span data-ttu-id="a3e7b-106">לחנות המרכזית של מדיניות קבוצתית בתחום של Active Directory, או לתיקיה תבנית הגדרת מדיניות במחשבים בודדים, התקן את כל תבניות הניהול המוסיפות כללים והגדרות עבור Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="a3e7b-106">To the Group Policy Central Store in your Active Directory domain, or to the Policy Definition template folder on individual computers, install all administrative templates that add rules and settings for Microsoft Edge.</span></span>
2. <span data-ttu-id="a3e7b-107">קבע את תצורת המדיניות הספציפית שברצונך להגדיר.</span><span class="sxs-lookup"><span data-stu-id="a3e7b-107">Configure the specific policies you want to set.</span></span>

<span data-ttu-id="a3e7b-108">לקבלת מידע נוסף, ראה [קביעת תצורה של הגדרות מדיניות Edge של Microsoft ב-Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span><span class="sxs-lookup"><span data-stu-id="a3e7b-108">To learn more, see [Configure Microsoft Edge policy settings on Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span></span>
