---
title: הפיכת Office 365 ATP לזמין עבור SharePoint, OneDrive ו- Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543929"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="67e0b-102">הפוך את Microsoft Defender לזמין Office 365 עבור SharePoint מקוון, OneDrive ו- Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="67e0b-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="67e0b-103">עבור https://protection.office.com אל והירשם.</span><span class="sxs-lookup"><span data-stu-id="67e0b-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="67e0b-104">בחר **קבצים מצורפים בטוחים**  >  **של** מדיניות ניהול  >  **איומים**.</span><span class="sxs-lookup"><span data-stu-id="67e0b-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="67e0b-105">בחר **הפעל את Defender עבור Office 365 עבור SharePoint, OneDrive ו- Microsoft Teams** ולאחר מכן לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="67e0b-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="67e0b-106">(מומלץ) כמנהל מערכת כללי או כמנהל מערכת SharePoint Online, הפעל [את cmdlet Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) עם **הפרמטר DisallowInfectedFileDownload** מוגדר ל- *true*.</span><span class="sxs-lookup"><span data-stu-id="67e0b-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="67e0b-107">(מומלץ) [הגדר התראות עבור](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) קבצים שזוהו.</span><span class="sxs-lookup"><span data-stu-id="67e0b-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="67e0b-108">Microsoft Defender עבור Office 365 לא יסרוק כל קובץ ב- SharePoint Online, OneDrive או Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="67e0b-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="67e0b-109">קבצים נסרקים באופן אסינכרוני, באמצעות תהליך המשתמש באירועי שיתוף ופעילות אורח, יחד עם הוריסטיקות חכמות ואותות איומים לזיהוי קבצים זדוניים.</span><span class="sxs-lookup"><span data-stu-id="67e0b-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="67e0b-110">עיין [ב- Microsoft Defender לקבלת Office 365 עבור SharePoint, OneDrive ו- Microsoft Teams.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)</span><span class="sxs-lookup"><span data-stu-id="67e0b-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>