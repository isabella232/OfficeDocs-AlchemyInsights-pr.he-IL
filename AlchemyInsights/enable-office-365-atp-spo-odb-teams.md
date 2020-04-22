---
title: אפשר ל-Office 365 ATP עבור SharePoint, OneDrive וצוותי Microsoft
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703427"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="1ad79-102">אפשר ל-Office 365 להגן על איום מתקדם עבור SharePoint Online, OneDrive וצוותי Microsoft</span><span class="sxs-lookup"><span data-stu-id="1ad79-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="1ad79-103">. היכנס https://protection.office.com והיכנס</span><span class="sxs-lookup"><span data-stu-id="1ad79-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="1ad79-104">בחר > **במדיניות** >  **ניהול האיומים\*\*\*\*קבצים מצורפים בטוחים**.</span><span class="sxs-lookup"><span data-stu-id="1ad79-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="1ad79-105">בחר **באפשרות הפעל את ה-ATP לצוותי SharePoint, OneDrive ו-Microsoft**ולאחר מכן לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="1ad79-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="1ad79-106">ומלץ כמנהל כללי או כמנהל מערכת של SharePoint Online, הפעל את יישומון ה [-Cmdlet Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) עם **הפרמטר** מוגדר כ- *true*.</span><span class="sxs-lookup"><span data-stu-id="1ad79-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="1ad79-107">ומלץ [הגדיר התראות](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) עבור קבצים שזוהו.</span><span class="sxs-lookup"><span data-stu-id="1ad79-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="1ad79-108">ATP יסרוק לסרוק כל קובץ בודד ב-SharePoint Online, OneDrive או בצוותי Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1ad79-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="1ad79-109">הקבצים נסרקים באופן אסינכרוני, באמצעות תהליך המשתמש באירועים של שיתוף ופעילות אורח, יחד עם היוריסטיקה חכמה ואותות איום כדי לזהות קבצים זדוניים.</span><span class="sxs-lookup"><span data-stu-id="1ad79-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="1ad79-110">ראה [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="1ad79-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>