---
title: אפשר ATP Office 365 עבור SharePoint, OneDrive ו- Microsoft צוותים
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/02/2019
ms.locfileid: "31030982"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="9ff26-102">אפשר Office 365 איום מתקדם הגנה עבור SharePoint במצב מקוון, OneDrive ו- Microsoft צוותים</span><span class="sxs-lookup"><span data-stu-id="9ff26-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="9ff26-103">עבור אל https://protection.office.com ולהיכנס.</span><span class="sxs-lookup"><span data-stu-id="9ff26-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="9ff26-104">בחר **ניהול איום** > **מדיניות** > **מסמכים מצורפים בטוחים**.</span><span class="sxs-lookup"><span data-stu-id="9ff26-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="9ff26-105">בחר **להפעיל ATP עבור SharePoint, OneDrive, ו- Microsoft צוותים**ולאחר מכן לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="9ff26-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="9ff26-106">(מומלץ) מנהל כללי או כמנהל SharePoint Online, להפעיל cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) עם הפרמטר **DisallowInfectedFileDownload** מוגדר כ- *true*.</span><span class="sxs-lookup"><span data-stu-id="9ff26-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="9ff26-107">(מומלץ) [הגדר התראות](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) עבור הקבצים שאותרו.</span><span class="sxs-lookup"><span data-stu-id="9ff26-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="9ff26-108">ATP יבצע סריקה nto כל קובץ בודד ב- SharePoint Online, OneDrive או צוותים של Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9ff26-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="9ff26-109">קבצים נסרקים באופן אסינכרוני, באמצעות תהליך העושה שימוש שיתוף מוזמנים פעילות ואירועי, יחד עם בהיריסטיקה חכמים ואת אותות איום כדי לזהות קבצים מזיקים.</span><span class="sxs-lookup"><span data-stu-id="9ff26-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="9ff26-110">ראה [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="9ff26-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>