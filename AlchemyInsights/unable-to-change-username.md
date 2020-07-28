---
title: אין אפשרות לשנות שם משתמש
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439551"
---
# <a name="unable-to-change-username"></a>אין אפשרות לשנות שם משתמש

במקרים מסוימים, השינויים ב-UPN (שם המשתמש) אינם מופצים לענן הצמתים. ייתכן שתקבל שגיאות אימות בפורטל של Office 365 או שלא תוכל לשנות את שם המשתמש או את כתובת הדואר האלקטרוני. כדי לפתור בעיה זו, הגדר באופן ידני את שם המשתמש באמצעות פקודה PowerShell זו.

**דוגמה: שינוי שם של משתמש**

PowerShellCopy

נ. ב.: \> Set-Msoluserהפריפלשם-מdavidc@contoso.com שם המשתמש "davidchew@contoso.com"

פקודה זו שינוי שם הdavidc@contoso.com לdavidchew@contoso.com.

לקבלת מידע נוסף, ראה [הגדרת משתמשים בשמות](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).