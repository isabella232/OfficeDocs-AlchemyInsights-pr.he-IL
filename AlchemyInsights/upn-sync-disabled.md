---
title: סינכרון UPN אינו זמין
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
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038113"
---
# <a name="upn-sync-disabled"></a>סינכרון UPN אינו זמין

אם התחלת לסנכרן עם Azure AD לפני 30 במרץ 2016, הפעל את cmdlet Azure AD PowerShell הבא כדי לאפשר התאמה רכה של UPN עבור הארגון שלך בלבד:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -enable $True**
  
התאמה רכה של UPN מופעלת באופן אוטומטי עבור ארגונים שהתחילו לסנכרן עם Azure AD ב- 30 במרץ 2016 או לאחר.
  
כדי ללמוד עוד אודות הפיכת התאמה רכה לכוללת ב- UPN ובתכונות סינכרון אחרות, ראה [Azure AD התחברות תכונות שירות הסינכרון](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

