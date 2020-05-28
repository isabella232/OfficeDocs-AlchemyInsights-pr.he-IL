---
title: ניהול משתמש מסונכרן
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
ms.openlocfilehash: 84e337a7224fdd3c3ab7ad0f61240692fe007d5a
ms.sourcegitcommit: 82af227ac6d075e748e27c4ce6bdcf56628559cb
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/28/2020
ms.locfileid: "44407351"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>אין אפשרות להגדיר כתובת דואר אלקטרוני ראשית, לשנות את תכונות המשתמש או להסיר/למחוק משתמש מסונכרן

אם סינכרון ספריות מאופשר עבור הסביבה שלך, לא ניתן לשנות תכונות מסוימות של משתמשים או אובייקטים באמצעות מרכז הניהול של Microsoft 365.

כדי לנהל באופן מלא משתמשים מסונכרנים ואת כל התכונות שלהם, השתמש במסוף הניהול של המשתמשים והקבוצות של הספריה המקומית (adsiedit. msc).  

לחלופין, באפשרותך לשנות משתמשים או תכונות בודדים עבור משתמשים מסונכרנים באמצעות powershell כגון המוצג בדוגמאות נפוצות אלה: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
