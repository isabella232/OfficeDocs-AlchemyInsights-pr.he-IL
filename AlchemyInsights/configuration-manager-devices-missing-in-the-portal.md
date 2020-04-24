---
title: מכשירים המשויכים למנהל התצורה אינם מופיעים בפורטל
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: 7a11ad3c6970be2c52a7cf0696bd3810b9bd665a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2020
ms.locfileid: "43789903"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="c3fc7-102">מכשירים המשויכים למנהל התצורה אינם מופיעים בפורטל</span><span class="sxs-lookup"><span data-stu-id="c3fc7-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="c3fc7-103">כדי שסינכרון המכשירים יפעל, חייבת להיות אפשרות גישה אל [נקודות הקצה האינטרנטיות הנדרשות](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) באמצעות השרת המקומי המארח את תפקיד נקודת החיבור לשירות.</span><span class="sxs-lookup"><span data-stu-id="c3fc7-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="c3fc7-104">כדי לפתור בעיות בסינכרון מכשירים, עיין בקובץ **CMGatewaySyncUploadWorker.log** הנמצא בנקודת החיבור לשירות.</span><span class="sxs-lookup"><span data-stu-id="c3fc7-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="c3fc7-105">קבל מידע נוסף אודות [צירוף דייר במנהל נקודות הקצה של Microsoft](https://docs.microsoft.com/configmgr/tenant-attach/).</span><span class="sxs-lookup"><span data-stu-id="c3fc7-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
