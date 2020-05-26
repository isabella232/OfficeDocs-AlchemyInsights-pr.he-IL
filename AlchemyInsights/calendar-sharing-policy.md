---
title: 618 מדיניות שיתוף לוח שנה
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373000"
---
# <a name="policy-error-when-sharing-a-calendar"></a>שגיאת מדיניות בעת שיתוף לוח שנה

1. בצע אחת מהפעולות הבאות, בהתאם למצבך:
    - התחבר ל-Exchange Online באמצעות מרחוק PowerShell. לקבלת מידע נוסף, ראה [התחברות ל-Exchange Online באמצעות מרחוק PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - בשרת המקומי, פתח את מעטפת ניהול Exchange.
2. קבע את מדיניות השיתוף שהוקצתה למשתמש. לשם כך, הפעל את הפקודה הבאה וציין את המדיניות המוחזרת:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. עדכן את מדיניות השיתוף עבור המשתמש. כדי לעשות זאת, בצע את הפעולות הבאות:
    - פתח את מרכז הניהול של Exchange.
    - לחץ על **ארגון**ולאחר מכן לחץ פעמיים על המדיניות שהוקצתה למשתמש תחת **שיתוף בודד**. זוהי המדיניות שהוחזרה בשלב 2.
    - בדף ' כלל שיתוף ', בחר ברמת שיתוף לוח השנה שברצונך לאפשר תחת **ציון איזה מידע ברצונך לשתף**; לחץ על **שמור**.

לקבלת מידע נוסף, ראה: ["מדיניות אינה מאפשרת הענקת הרשאות ברמה זו לאחת או יותר מבין הנמענים" כאשר המשתמש מנסה לשתף לוח שנה](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
