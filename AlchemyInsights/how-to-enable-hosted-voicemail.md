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
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318649"
---
# <a name="how-to-enable-hosted-voicemail"></a>כיצד להפוך דואר קולי מתארח לזמין

כדי להפוך דואר קולי **לזמין, HostedVoicemail** חייב להיות מוגדר $true.

המאפיין **HostedVoicemail** על המשתמש באמצעות PowerShell מרוחק (RPS).

לקבלת מידע נוסף אודות התחברות ל- RPS, [ראה Microsoft Teams PowerShell מבט](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) כולל לקבלת מידע נוסף אודות התחברות ל- RPS.

1. מנהל Teams צריך להיכנס ל- PowerShell מרוחק עבור Teams.
1. מתוך שורת הפקודה של PowerShell Teams מנהל המערכת יכול להפעיל **את set-csuser user@contoso.com -HostedVoiceMail $true** שבו sip uri הוא של המשתמש הנושאל.

**הערה:** שינויים במדיניות יכולים לאסוף עד 24 שעות לשכפול.