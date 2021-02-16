---
title: הפיכת התקן לזמין
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8278"
ms.openlocfilehash: 9e4b03dcba7a2c98a5d63213ee49f9ba8f91d670
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256869"
---
# <a name="enable-device"></a><span data-ttu-id="3f578-102">הפיכת התקן לזמין</span><span class="sxs-lookup"><span data-stu-id="3f578-102">Enable Device</span></span>

<span data-ttu-id="3f578-103">**כדי להפוך את ההתקן לזמין באמצעות הפקודה Powershell**</span><span class="sxs-lookup"><span data-stu-id="3f578-103">**To enable the device using Powershell command**</span></span>

<span data-ttu-id="3f578-104">הפעל את הפקודות הבאות:</span><span class="sxs-lookup"><span data-stu-id="3f578-104">Run the following commands:</span></span>

- <span data-ttu-id="3f578-105">כדי לקבל את אובייקט ההתקן: `Get-MsolDevice -Name <Name>`</span><span class="sxs-lookup"><span data-stu-id="3f578-105">To get device object: `Get-MsolDevice -Name <Name>`</span></span>
- <span data-ttu-id="3f578-106">כדי לאפשר התקן: `Enable-MsolDevice -DeviceId <DeviceId>`</span><span class="sxs-lookup"><span data-stu-id="3f578-106">To enable device: `Enable-MsolDevice -DeviceId <DeviceId>`</span></span>

<span data-ttu-id="3f578-107">לקבלת מידע נוסף אודות קביעת התצורה של הצטרפות היברידית בתחומים מנוהלים, ראה [קביעת תצורה של הצטרפות משולבת](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains).</span><span class="sxs-lookup"><span data-stu-id="3f578-107">For more information on Configuring Hybrid Join on managed domains, see [Configure Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains).</span></span>
