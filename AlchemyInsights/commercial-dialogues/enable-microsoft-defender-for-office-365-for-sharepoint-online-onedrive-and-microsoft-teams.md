---
title: הפיכת Microsoft Defender לזמין עבור Office 365 עבור SharePoint Online, OneDrive ו-Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745305"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="e2656-102">הפיכת Microsoft Defender לזמין עבור Office 365 עבור SharePoint Online, OneDrive ו-Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="e2656-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive and Microsoft Teams</span></span>

1. <span data-ttu-id="e2656-103">באמצעות אישורי מנהל המערכת הכלליים או מנהל האבטחה שלך, היכנס [למרכז האבטחה והתאימות של Office 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="e2656-103">Using your global admin or security admin credentials, log in to the [Office 365 Security and Compliance Center](https://protection.office.com/).</span></span>
2. <span data-ttu-id="e2656-104">בחר **ניהול סיכונים** בחלונית הימנית ולאחר מכן בחר באפשרות קבצים מצורפים בטוחים **של מדיניות**  >  [](https://protection.office.com/safeattachment).</span><span class="sxs-lookup"><span data-stu-id="e2656-104">Select **Threat management** in the left pane, and then select **Policy** > [Safe attachments](https://protection.office.com/safeattachment).</span></span>
3. <span data-ttu-id="e2656-105">בחר **הפעל את Microsoft Defender עבור Office 365 עבור SharePoint, OneDrive ו-Microsoft teams** ולאחר מכן בחר **שמור**.</span><span class="sxs-lookup"><span data-stu-id="e2656-105">Select **Turn on Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then select **Save**.</span></span>
    > [!TIP]
    >
    > - <span data-ttu-id="e2656-106">כמנהל מערכת כללי או כמנהל מערכת של SharePoint Online, הגדר את ה-cmdlet הבא של PowerShell כאשר הפרמטר **DisallowInfectedFileDownload** מוגדר ל- *true*: [set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span><span class="sxs-lookup"><span data-stu-id="e2656-106">As a global admin or a SharePoint Online admin, run the following PowerShell cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span></span>
    > - [<span data-ttu-id="e2656-107">הגדרת התראות עבור קבצים שזוהו</span><span class="sxs-lookup"><span data-stu-id="e2656-107">Set up alerts for detected files</span></span>](https://go.microsoft.com/fwlink/?linkid=2092110)

<span data-ttu-id="e2656-108">לקבלת מידע נוסף, ראה [Microsoft Defender עבור Office 365 עבור SharePoint, OneDrive ו-Microsoft teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span><span class="sxs-lookup"><span data-stu-id="e2656-108">For more information, see [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span></span>
