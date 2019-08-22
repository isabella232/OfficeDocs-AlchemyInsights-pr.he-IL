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
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36541996"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>אין אפשרות להגדיר כתובת דואר אלקטרוני ראשית או לשנות תכונות משתמש

אם סינכרון ספריות זמין עבור הסביבה שלך, אין אפשרות לשנות תכונות מסוימות למשתמש או לאובייקט Microsoft 365 admin למרכז.

כדי לנהל באופן מלא כל התכונות שלהם ומשתמשים מסונכרן, השתמש שלך אקטיבית מקומיים משתמשים וקבוצות במסוף ניהול (adsiedit.msc).  

לחלופין, באפשרותך לשנות משתמשים בודדים או תכונות עבור משתמשים מסונכרנים באמצעות powershell כגון שמוצג בדוגמאות אלה נפוצים: 
- ערכת-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- ערכת-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "משתמש בדיקה" - שם משפחה "משתמש"-כותרת "Manager"-מחלקה "משאבי אנוש"
- הסר-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com