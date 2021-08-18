---
title: שגיאת רישוי DLP של נקודת קצה
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200001"
- "7176"
ms.openlocfilehash: c32ab88a72c265be411350e50756f5b2e1e3337c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322132"
---
# <a name="endpoint-dlp-licensing-error"></a>שגיאת רישוי DLP של נקודת קצה

בעת ניסיון להגדיר DLP של נקודת קצה, אם אתה מקבל את השגיאה הבאה:

`Your organization is missing the licenses required to manage these devices`.

ודא שיש לך אחד מהנויי או ההרחבות הבאים:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Microsoft 365 E5 עמידה בדרישות
- Microsoft 365 A5 תאימות
- Microsoft 365 E5 מידע ופיקוח
- Microsoft 365 A5 מידע ופיקוח

**הערה:** פעולה זו לא תעבד עבור שילובי רשיונות, כמו: Win E5 + O365 E5 + EMS E5. כדי להגדיר תכונה זו, עליך להיות בעל רשיון M365 E5 טהור.

לקבלת מידע נוסף אודות רישוי DLP של נקודות קצה, [ראה רישוי DLP של נקודת קצה.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
