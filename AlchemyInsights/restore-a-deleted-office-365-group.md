---
title: שחזור קבוצה שנמחקה של Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645132"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>שחזור קבוצה שנמחקה של Microsoft 365

באפשרותך לשחזר קבוצה שנמחקה של Microsoft 365 או Microsoft Teams תוך 30 יום ממחיקתה.

1. עבור אל מרכז הניהול של [Microsoft 365](https://aka.ms/RestoreDeletedGroup) כדי להיכנס לרשימה של הקבוצות והצוותים שנמחקו.

    **הערה:** היכנס באמצעות החשבון שהוקצה למנהל הדייר או לתפקיד מנהל המערכת של הקבוצות.

1. בחר את הקבוצה/Teams שנמחקה כדי לשחזר ולחץ על **שחזר את הקבוצה**.

    אם לא ניתן לשחזר את הקבוצה עקב כתובת SMTP מתנגשת, השתמש בפקודה הבאה כדי למצוא את האובייקט הגורם להתנגשות ולהסיר את כתובת ה- SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **הערה:** במקרים מסוימים, ייתכן שיקח עד 24 שעות עד שהקבוצה וכל הנתונים שלה ישוחזרו.

    לקבלת מידע נוסף, או כדי ללמוד כיצד לשחזר קבוצות באמצעות PowerShell, ראה [שחזור קבוצה שנמחקה של Microsoft 365](https://go.microsoft.com/fwlink/?linkid=867802).