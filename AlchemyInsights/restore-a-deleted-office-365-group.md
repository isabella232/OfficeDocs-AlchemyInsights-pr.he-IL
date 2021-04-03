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
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505687"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>שחזור קבוצה שנמחקה של Microsoft 365

באפשרותך לשחזר קבוצה שנמחקה של Microsoft 365 או Microsoft Teams תוך 30 יום ממחיקתה.

1. כדי להיכנס למרכז הניהול של Microsoft 365 ולרשימת הקבוצות והצוותים שנמחקו, עבור אל [מרכז הניהול של Microsoft 365](https://aka.ms/RestoreDeletedGroup).

    **הערה:** היכנס באמצעות החשבון שהוקצה למנהל הדייר או לתפקיד מנהל המערכת של הקבוצות.

1. בחר את הקבוצה/Teams שנמחקה כדי לשחזר ולחץ על **שחזר את הקבוצה**.

    אם לא ניתן לשחזר את הקבוצה עקב כתובת SMTP מתנגשת, השתמש בפקודה הבאה כדי למצוא את האובייקט הגורם להתנגשות ולהסיר את כתובת ה- SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **הערה:** במקרים מסוימים, ייתכן שיקח עד 24 שעות עד שהקבוצה וכל הנתונים שלה ישוחזרו.

    לקבלת מידע נוסף, או כדי ללמוד כיצד לשחזר קבוצות באמצעות PowerShell, ראה [שחזור קבוצה שנמחקה של Microsoft 365](https://go.microsoft.com/fwlink/?linkid=867802).