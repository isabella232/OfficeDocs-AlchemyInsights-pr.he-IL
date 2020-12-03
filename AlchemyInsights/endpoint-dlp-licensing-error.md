---
title: שגיאת רישוי של נקודת קצה של DLP
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
ms.openlocfilehash: d17c51177898d62c7c477460c8c26b4753bae65f
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564609"
---
# <a name="endpoint-dlp-licensing-error"></a>שגיאת רישוי של נקודת קצה של DLP

בעת ניסיון להגדיר DLP של נקודת קצה, אם אתה מקבל את השגיאה הבאה:

`Your organization is missing the licenses required to manage these devices`.

ודא שברשותך אחד מהמנויים או התוספות הבאים:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- תאימות ל-Microsoft 365 E5
- תאימות של Microsoft 365 A5
- Microsoft 365 E5 הגנה וממשל מידע
- Microsoft 365 A5 הגנה וממשל

> [!NOTE]
> פעולה זו לא תפעל עבור שילובי רשיונות כגון: Win E5 + O365 E5 + EMS E5. דרוש לך רשיון M365 E5 נקי כדי להגדיר תכונה זו.

לקבלת מידע נוסף בנוגע לרישוי של DLP, ראה [רישוי של נקודת קצה של dlp.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
