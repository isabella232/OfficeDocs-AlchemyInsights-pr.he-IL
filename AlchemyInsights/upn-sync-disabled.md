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
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782152"
---
# <a name="upn-sync-disabled"></a>סינכרון UPN אינו זמין

אם התחלת לסנכרן עם Azure AD לפני 30 במרץ 2016, הפעל את cmdlet Azure AD PowerShell הבא כדי לאפשר התאמה רכה של UPN עבור הארגון שלך בלבד:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -enable $True**
  
התאמה רכה של UPN מופעלת באופן אוטומטי עבור ארגונים שהתחילו לסנכרן עם Azure AD ב- 30 במרץ 2016 או לאחר.
  
כדי ללמוד עוד אודות הפיכת התאמה רכה ל אפשרית ב- UPN ובתכונות סינכרון אחרות, ראה [תכונות שירות הסינכרון של Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

