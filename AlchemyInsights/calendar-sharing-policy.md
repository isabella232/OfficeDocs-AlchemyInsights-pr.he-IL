---
title: מדיניות שיתוף לוח שנה 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091604"
---
# <a name="policy-error-when-sharing-a-calendar"></a>שגיאת מדיניות בעת שיתוף לוח שנה

1. עשה אחת מהפעולות הבאות, בהתאם למצב שלך:
    - התחברות כדי Exchange Online באמצעות PowerShell מרוחק. לקבלת מידע נוסף, [ראה התחברות כדי Exchange Online ב- PowerShell מרוחק](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - בשרת המקומי, פתח את מעטפת Exchange הניהול.
2. קבע את מדיניות השיתוף שהוקצתה למשתמש. לשם כך, הפעל את הפקודה הבאה ורשום את המדיניות שהוחזרה:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. עדכן את מדיניות השיתוף עבור המשתמש. לשם כך, בצע את הפעולות הבאות:
    - פתח את Exchange הניהול של התמיכה.
    - לחץ **על** ארגון ולאחר מכן לחץ פעמיים על המדיניות שהוקצתה למשתמש תחת **שיתוף בודד**. זוהי המדיניות שהוחזרה בשלב 2.
    - בדף כלל שיתוף, בחר את רמת שיתוף לוח השנה שברצונך לאפשר תחת ציין **איזה מידע ברצונך לשתף;** לחץ **על שמור**.

לקבלת מידע נוסף, ראה: "מדיניות אינה מאפשרת הענקת הרשאות ברמה זו לשגיאה אחת או יותר מהנמענים" כאשר המשתמש [מנסה לשתף לוח שנה.](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)
