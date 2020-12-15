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
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/09/2020
ms.locfileid: "49678000"
---
# <a name="how-to-enable-hosted-voicemail"></a>כיצד להפוך דואר קולי מתארח לזמין

כדי להפוך את הדואר הקולי לזמין, **HostedVoicemail** חייב להיות מוגדר ל$true.

המאפיין **HostedVoicemail** במשתמש שמשתמש ב-PowerShell מרוחק (RPS).

לקבלת מידע נוסף אודות התחברות ל-RPS, ראה [מבט כולל על Microsoft teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) לקבלת מידע נוסף אודות התחברות ל-RPS.

1. מנהל הצוותים אמור להיות מחובר ל-PowerShell מרוחק עבור Teams.
1. מ-PowerShell הצג בקשה למנהל הצוותים להפעיל את **set-csuser user@contoso.com-HostedVoiceMail $true** שבו המשתמש של sip הוא המשתמש הנדון.

> [!NOTE]
> שינויים בפריטי מדיניות יכולים להימשך עד 24 שעות כדי לשכפל.