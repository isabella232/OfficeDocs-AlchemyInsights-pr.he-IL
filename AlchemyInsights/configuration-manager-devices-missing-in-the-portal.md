---
title: מכשירים המשויכים למנהל התצורה אינם מופיעים בפורטל
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: d57659eb928dd8c4653499e65b6e6cd2f021f521
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817245"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>מכשירים המשויכים למנהל התצורה אינם מופיעים בפורטל

כדי שסינכרון המכשירים יפעל, חייבת להיות אפשרות גישה אל [נקודות הקצה האינטרנטיות הנדרשות](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) באמצעות השרת המקומי המארח את תפקיד נקודת החיבור לשירות. כדי לפתור בעיות בסינכרון מכשירים, עיין בקובץ **CMGatewaySyncUploadWorker.log** הנמצא בנקודת החיבור לשירות.

קבל מידע נוסף אודות [צירוף דייר במנהל נקודות הקצה של Microsoft](https://docs.microsoft.com/configmgr/tenant-attach/).
