---
title: הגדרת ClientAccessServerEnabled ל- True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: fc953813a94c9ed3226f81f776d6085e12a6cafc
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320357"
---
# <a name="set-clientaccessserverenabled-to-true"></a>הגדרת ClientAccessServerEnabled ל- True

אם אינך יכול לפתוח הודעת דואר אלקטרוני מוצפנת ובמקום זאת לראות קובץ **מצורף של rpmsg,** בצע את השלבים הבאים:

1. התחברות כדי Exchange Online PowerShell.

    **הערה**: כדי להתחבר Exchange Online PowerShell, עליך להיכנס באמצעות מנהל מערכת כללי או Exchange מנהל מערכת.

   a. פתח Windows PowerShell ולאחר מכן הפעל את הפקודה הבאה:`$UserCredential = Get-Credential`
   b. בתיבת **הדו-שיח Windows PowerShell אישור,** הזן את החשבון והסיסמה שלך בעבודה או בבית הספר, ג. לחץ על **אישור**. 

2. הפעל את הפקודה הבאה כדי ליצור הפעלה חדשה:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. הפעל את הפקודה הבאה:
    
    `Import-PSSession $Session -DisableNameChecking`

3. הפקודה `Get-IRMConfiguration` הפעל.

4. בדוק את **ההגדרה ClientAccessServerEnabled.** 

    a. אם **ההגדרה ClientAccessServerEnabled** מוגדרת ל- **False**, הפעל את ה- cmdlet הבא: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

**עצה**: סגור תמיד את הפעלת Powershell באמצעות הפקודה הבאה: `Remove-PSSession $Session`

לקבלת מידע נוסף, [ראה Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

