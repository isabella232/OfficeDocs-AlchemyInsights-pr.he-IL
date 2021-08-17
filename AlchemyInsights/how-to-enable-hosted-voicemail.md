---
title: כיצד להפוך דואר קולי מתארח לזמין
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055555"
---
# <a name="how-to-enable-hosted-voicemail"></a>כיצד להפוך דואר קולי מתארח לזמין

כדי להפוך דואר קולי **לזמין, HostedVoicemail** חייב להיות מוגדר $true.

המאפיין **HostedVoicemail** על המשתמש באמצעות PowerShell מרוחק (RPS).

לקבלת מידע נוסף אודות התחברות ל- RPS, [ראה Microsoft Teams PowerShell מבט](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) כולל לקבלת מידע נוסף אודות התחברות ל- RPS.

1. מנהל Teams צריך להיכנס ל- PowerShell מרוחק עבור Teams.
1. מ- PowerShell, Teams מנהל המערכת יכול להפעיל **את set-csuser user@contoso.com -HostedVoiceMail $true** שבו sip uri הוא של המשתמש הנוהל.

> [!NOTE]
> השכפול של שינויים במדיניות עשוי לאסוף עד 24 שעות.