---
title: שחזור קבוצת Microsoft 365 שנמחקה
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
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959027"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>שחזור קבוצת Microsoft 365 שנמחקה

באפשרותך לשחזר קבוצה Microsoft 365 או Microsoft Teams תוך 30 יום ממחיקתה.

1. עבור אל [מרכז הניהול של Microsoft 365](https://aka.ms/RestoreDeletedGroup) כדי להיכנס לרשימה של הקבוצות והצוותים שנמחקו.

    **הערה:** היכנס באמצעות החשבון שהוקצה למנהל הדייר או לתפקיד מנהל המערכת של הקבוצות.

1. בחר את הקבוצה Microsoft 365/Teams כדי לשחזר ולחץ על **שחזר קבוצה**.

    אם לא ניתן לשחזר את הקבוצה עקב כתובת SMTP מתנגשת, השתמש בפקודה הבאה כדי למצוא את האובייקט הגורם להתנגשות ולהסיר את כתובת ה- SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **הערה:** במקרים מסוימים, ייתכן שיקח עד 24 שעות עד שהקבוצה וכל הנתונים שלה ישוחזרו.

    לקבלת מידע נוסף, או כדי ללמוד כיצד לשחזר קבוצות באמצעות PowerShell, ראה [שחזור קבוצת Microsoft 365 שנמחקה](https://go.microsoft.com/fwlink/?linkid=867802).