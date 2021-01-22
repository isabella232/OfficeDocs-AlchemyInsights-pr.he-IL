---
title: הפעלת טכנולוגיית NDI
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
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935102"
---
# <a name="turn-on-ndi-technology"></a>הפעלת טכנולוגיית NDI

טכנולוגיית NDI מחייבת שני שלבים להיות מופעלים עבור משתמש:

1. מנהל הדיירים חייב להפוך את המאפיין ' AllowNDIStreaming ' לזמין ב-CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. לאחר האכלוס של שינוי זה, משתמש הקצה חייב להפעיל את טכנולוגיית NDI® עבור הלקוח הספציפי שלו מתוך **הרשאות > הגדרות**.

לקבלת מידע נוסף, ראה [שימוש בטכנולוגיית NDI ב-Microsoft teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).
