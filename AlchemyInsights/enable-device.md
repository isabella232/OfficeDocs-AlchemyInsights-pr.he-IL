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
# <a name="enable-device"></a>הפיכת התקן לזמין

**כדי להפוך את ההתקן לזמין באמצעות הפקודה Powershell**

הפעל את הפקודות הבאות:

- כדי לקבל את אובייקט ההתקן: `Get-MsolDevice -Name <Name>`
- כדי לאפשר התקן: `Enable-MsolDevice -DeviceId <DeviceId>`

לקבלת מידע נוסף אודות קביעת התצורה של הצטרפות היברידית בתחומים מנוהלים, ראה [קביעת תצורה של הצטרפות משולבת](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains).
