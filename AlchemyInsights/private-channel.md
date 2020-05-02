---
title: ערוץ פרטי
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005439"
---
# <a name="private-channels-in-microsoft-teams"></a>ערוצים פרטיים בצוותי Microsoft

ערוצים פרטיים הם תכונה חדשה בצוותי Microsoft. שים לב שאין אפשרות להמיר ערוצים פרטיים מערוצים רגילים או להיפך.

לקבלת פרטים אודות ערוצים פרטיים, כגון מידע אודות [יצירת ערוצים פרטיים ואתרי](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) [SharePoint של ערוצים](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites)פרטיים, ראה [ערוצים פרטיים בצוותי Microsoft](https://docs.microsoft.com/MicrosoftTeams/private-channels). 

**הערה:** מאחר שתצורה עבור שמירה של הודעות ערוץ פרטי אינה נתמכת עדיין, לדיירים עם מדיניות שמירה מאופשרת לא יהיו ערוצים פרטיים הזמינים כברירת מחדל. ניתן להפעיל ערוצים פרטיים במרכז הניהול של הצוותים. בנוסף, שים לב שבזמן שמירה של הודעות ערוץ פרטי אינה נתמכת, קיימת תמיכה בשמירה של קבצים המשותפים בערוצים פרטיים.

**צריך בעל צוות חדש?**

אם בעל הערוץ הפרטי שלך עוזב, באפשרותך להוסיף בעל צוות חדש דרך צוותי Powershell.


- לך [לכאן](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) כדי להתקין את הצוותים Powershell.

להלן יישומון ה-cmdlet הדרוש לך:

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

לקבלת מידע נוסף על צוותי Powershell, ראה [קבוצות מבט כולל על powershell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).
