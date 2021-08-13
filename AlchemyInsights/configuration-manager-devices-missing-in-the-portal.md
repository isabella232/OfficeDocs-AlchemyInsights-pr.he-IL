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
ms.openlocfilehash: 358bb6aa0420a845e51e0b75049c2ae790daf3690e5cfb115b234d82a29e93a7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966110"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>מכשירים המשויכים למנהל התצורה אינם מופיעים בפורטל

כדי שסינכרון המכשירים יפעל, חייבת להיות אפשרות גישה אל [נקודות הקצה האינטרנטיות הנדרשות](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) באמצעות השרת המקומי המארח את תפקיד נקודת החיבור לשירות. כדי לפתור בעיות בסינכרון מכשירים, עיין בקובץ **CMGatewaySyncUploadWorker.log** הנמצא בנקודת החיבור לשירות.

קבל מידע נוסף אודות [צירוף דייר במנהל נקודות הקצה של Microsoft](https://docs.microsoft.com/configmgr/tenant-attach/).
