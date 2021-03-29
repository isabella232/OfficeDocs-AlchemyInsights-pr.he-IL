---
title: קביעת תצורה של הגדרות מדיניות Microsoft Edge ב- Windows
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
- "9004632"
- "6894"
- "8358"
ms.openlocfilehash: e9bb489b4d8ecd76fd777ade9fb740ecad542900
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402376"
---
# <a name="configure-microsoft-edge-policy-settings-on-windows"></a><span data-ttu-id="f1d1d-102">קביעת תצורה של הגדרות מדיניות Microsoft Edge ב- Windows</span><span class="sxs-lookup"><span data-stu-id="f1d1d-102">Configure Microsoft Edge policy settings on Windows</span></span>

<span data-ttu-id="f1d1d-103">כדי לקבוע את התצורה של הגדרות מדיניות ועדכונים מנוהלים עבור Microsoft Edge, השתמש באובייקטי מדיניות קבוצתית (GPO).</span><span class="sxs-lookup"><span data-stu-id="f1d1d-103">To configure policy settings and managed updates for Microsoft Edge, use Group Policy Objects (GPOs).</span></span> <span data-ttu-id="f1d1d-104">באפשרותך גם להקצות מדיניות באמצעות הרישום; פעולה זו מתאימה עבור (1) מכשירי Windows המצורפים לתחום של Microsoft Active Directory ולמופעי Windows 10 Pro ו- Enterprise שנרשמו לניהול מכשירים ב- Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="f1d1d-104">You can also provision policy through the registry; this would be appropriate for (1) Windows devices joined to a Microsoft Active Directory domain and for (2) Windows 10 Pro and Enterprise instances enrolled for device management in Microsoft Intune.</span></span>

<span data-ttu-id="f1d1d-105">כדי לקבוע את התצורה של Microsoft Edge באמצעות אובייקטי GPO, עשה את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="f1d1d-105">To configure Microsoft Edge by using GPOs, do the following:</span></span>

1. <span data-ttu-id="f1d1d-106">עבור אל החנות המרכזית של המדיניות הקבוצתית בתחום Active Directory שלך, או אל התיקיה תבנית הגדרת מדיניות במחשבים בודדים, התקן את כל תבניות הניהול המוסיפות כללים והגדרות עבור Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="f1d1d-106">Go to the Group Policy Central Store in your Active Directory domain, or to the Policy Definition template folder on individual computers, install all administrative templates that add rules and settings for Microsoft Edge.</span></span>
2. <span data-ttu-id="f1d1d-107">קבע את תצורת פריטי המדיניות הספציפיים שברצונך להגדיר.</span><span class="sxs-lookup"><span data-stu-id="f1d1d-107">Configure the specific policies you want to set.</span></span>

<span data-ttu-id="f1d1d-108">כדי ללמוד עוד, ראה קביעת [תצורה של הגדרות מדיניות Microsoft Edge ב- Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span><span class="sxs-lookup"><span data-stu-id="f1d1d-108">To learn more, see [Configure Microsoft Edge policy settings on Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span></span>
