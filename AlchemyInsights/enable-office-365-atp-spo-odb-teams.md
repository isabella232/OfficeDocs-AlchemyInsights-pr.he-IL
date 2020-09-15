---
title: הפיכת Office 365 ATP לזמין עבור SharePoint, OneDrive ו-Microsoft Teams
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
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709908"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="604eb-102">הפעלת הגנת האיום המתקדמת של Office 365 עבור SharePoint Online, OneDrive ו-Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="604eb-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="604eb-103">עבור אל https://protection.office.com והיכנס.</span><span class="sxs-lookup"><span data-stu-id="604eb-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="604eb-104">בחר **Threat management**  >  **Policy**  >  **קבצים מצורפים בטוחים במדיניות**ניהול האיום.</span><span class="sxs-lookup"><span data-stu-id="604eb-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="604eb-105">בחר **הפעל את ATP עבור SharePoint, OneDrive ו-Microsoft teams**ולאחר מכן לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="604eb-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="604eb-106">מומלץ כמנהל מערכת כללי או כמנהל מערכת של SharePoint Online, הגדר את ה [-Cmdlet set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) כאשר הפרמטר **DisallowInfectedFileDownload** מוגדר ל- *true*.</span><span class="sxs-lookup"><span data-stu-id="604eb-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="604eb-107">מומלץ [הגדרת התראות](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) עבור קבצים שזוהו.</span><span class="sxs-lookup"><span data-stu-id="604eb-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="604eb-108">ATP יופיע כדי לסרוק כל קובץ בודד ב-SharePoint Online, ב-OneDrive או ב-Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="604eb-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="604eb-109">הקבצים נסרקים באופן אסינכרוני, באמצעות תהליך המשתמש באירועים של שיתוף ופעילויות אורח, יחד עם היישויות חכמות ואותות איום כדי לזהות קבצים זדוניים.</span><span class="sxs-lookup"><span data-stu-id="604eb-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="604eb-110">ראה [ATP עבור SharePoint, OneDrive ו-Microsoft teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="604eb-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>