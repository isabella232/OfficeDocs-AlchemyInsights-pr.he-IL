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
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023523"
---
# <a name="turn-on-ndi-technology"></a>הפעלת טכנולוגיית NDI

טכנולוגיית NDI דורשת הפעלה של שני שלבים עבור משתמש:

1. מנהל הדייר חייב להפוך את המאפיין 'AllowNDIStreaming' לזמין ב- CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. לאחר ששינוי זה מאוכלס, משתמש הקצה חייב להפעיל את טכנולוגיית NDI® עבור הלקוח הספציפי שלו **מתוך הגדרות > הרשאות.**

לקבלת מידע נוסף, ראה [שימוש בטכנולוגיית NDI ב- Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).
