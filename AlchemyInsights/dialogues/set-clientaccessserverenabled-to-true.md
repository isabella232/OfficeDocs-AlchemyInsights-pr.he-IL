---
title: הגדרת ClientAccessServerEnabled ל-True
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
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524556"
---
# <a name="set-clientaccessserverenabled-to-true"></a>הגדרת ClientAccessServerEnabled ל-True

אם אינך מצליח לפתוח הודעת דואר אלקטרוני מוצפנת ובמקום זאת אתה רואה קובץ מצורף של **rpmsg** , בצע את השלבים הבאים:

1. התחבר אל Exchange Online PowerShell.

> [!NOTE]
> כדי להתחבר ל-Exchange Online PowerShell, עליך להיכנס באמצעות חשבון מנהל מערכת כללי או מנהל מערכת של Exchange.

   מ. פתח את Windows PowerShell ולאחר מכן הפעלת הפקודה הבאה: `$UserCredential = Get-Credential`
b. בתיבת הדו **בקשת אישור של Windows PowerShell** , הזן את החשבון שלך בעבודה או בבית הספר והסיסמה שלך, c. לחץ על **אישור**. 

2. הפעלת הפקודה הבאה כדי ליצור הפעלה חדשה:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    מ. הפעל את הפקודה הבאה:
    
    `Import-PSSession $Session -DisableNameChecking`

3. הפקודה ' ההפעלה `Get-IRMConfiguration` '.

4. סמן את ההגדרה **ClientAccessServerEnabled** . 

    מ. אם ההגדרה **ClientAccessServerEnabled** מוגדרת ל- **False**, הפעלת את ה-cmdlet הבא: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> סגור תמיד את הפעלת powershell באמצעות הפקודה הבאה: `Remove-PSSession $Session`

לקבלת מידע נוסף, ראה [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

