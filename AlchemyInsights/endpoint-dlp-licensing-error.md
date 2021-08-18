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
ms.openlocfilehash: 1e242abe18717e5ef64d6f067ab3ec6fa8833cb672dd21c85e577ce640240ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090142"
---
# <a name="endpoint-dlp-licensing-error"></a>שגיאת רישוי DLP של נקודת קצה

בעת ניסיון להגדיר DLP של נקודת קצה, אם אתה מקבל את השגיאה הבאה:

`Your organization is missing the licenses required to manage these devices`.

ודא שיש לך אחד מהנויי או ההרחבות הבאים:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Microsoft 365 E5 תאימות
- Microsoft 365 A5 תאימות
- Microsoft 365 E5 מידע ופיקוח
- Microsoft 365 A5 מידע ופיקוח

> [!NOTE]
> פעולה זו לא תעבד עבור שילובי רשיונות, כמו: Win E5 + O365 E5 + EMS E5. כדי להגדיר תכונה זו, עליך להיות בעל רשיון M365 E5 טהור.

לקבלת מידע נוסף אודות רישוי DLP של נקודות קצה, [ראה רישוי DLP של נקודת קצה.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
