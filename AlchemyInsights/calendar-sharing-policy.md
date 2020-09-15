---
title: מדיניות שיתוף לוח שנה של 618
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
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684231"
---
# <a name="policy-error-when-sharing-a-calendar"></a>שגיאת מדיניות בעת שיתוף לוח שנה

1. בצע אחת מהפעולות הבאות, בהתאם למצב שלך:
    - התחבר ל-Exchange Online באמצעות PowerShell מרוחק. לקבלת מידע נוסף, ראה [התחברות ל-Exchange Online באמצעות PowerShell מרוחק](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - בשרת המקומי, פתח את מעטפת ניהול Exchange.
2. קבע את מדיניות השיתוף שהוקצתה למשתמש. לשם כך, הפעלת הפקודה הבאה ושימו לב למדיניות המוחזרת:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. עדכן את מדיניות השיתוף עבור המשתמש. לשם כך, בצע את הפעולות הבאות:
    - פתח את מרכז הניהול של Exchange.
    - לחץ על **ארגון**ולאחר מכן לחץ פעמיים על המדיניות שהוקצתה למשתמש תחת **שיתוף בודד**. זוהי המדיניות שהוחזרה בשלב 2.
    - בדף כלל שיתוף, בחר את רמת השיתוף של לוח השנה שברצונך לאפשר תחת **ציין איזה מידע ברצונך לשתף**; לחץ על **שמור**.

לקבלת מידע נוסף, ראה: ["מדיניות אינה מאפשרת הענקת הרשאות ברמה זו לשגיאה אחת או יותר של הנמענים" כאשר המשתמש מנסה לשתף לוח שנה](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
