---
title: ניהול המשתמש מסונכרן
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380506"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>אין אפשרות להגדיר כתובת דואר אלקטרוני ראשית או לשנות תכונות משתמש

אם סינכרון ספריות זמין עבור הסביבה שלך אין אפשרות לשנות תכונות מסוימות למשתמש או לאובייקט מרכז Admin.
כדי לנהל באופן מלא כל התכונות שלהם ומשתמשים מסונכרן, השתמש שלך אקטיבית מקומיים משתמשים וקבוצות במסוף ניהול (adsiedit.msc).  

לחלופין, באפשרותך לשנות משתמשים בודדים או תכונות עבור משתמשים מסונכרנים באמצעות powershell כגון שמוצג בדוגמאות אלה נפוצים: 
- ערכת-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- ערכת-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "משתמש בדיקה" - שם משפחה "משתמש"-כותרת "Manager"-מחלקה "משאבי אנוש"
- הסר-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com