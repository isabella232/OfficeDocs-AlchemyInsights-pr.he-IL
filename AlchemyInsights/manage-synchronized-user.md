---
title: ניהול משתמש מסונכרן
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 7bf7d3f00308ff6bc973cd52e09ca51c5fd0f45b
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451401"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>לא ניתן להגדיר את כתובת הדואר האלקטרוני הראשית, לשנות את תכונות המשתמש או להסיר/למחוק משתמש מסונכרן

אם סינכרון מדריכי כתובות זמין עבור הסביבה שלך, אין אפשרות לשנות תכונות מסוימות של משתמשים או אובייקטים באמצעות מרכז הניהול של Microsoft 365.

כדי לנהל באופן מלא משתמשים מסונכרנים ואת כל התכונות שלהם, השתמש במסוף ניהול הקבוצות והקבוצות המקומי של active directory (adsiedit. msc).  

לחלופין, באפשרותך לשנות משתמשים או תכונות בודדים עבור משתמשים מסונכרנים באמצעות powershell כגון המוצג בדוגמאות נפוצות אלה:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
