---
title: סינכרון UPN זמין
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 027782bb2a6b892df6201f3c3bf55151ef7b9db7
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657972"
---
# <a name="upn-sync-disabled"></a>סינכרון UPN זמין

אם התחלת סינכרון AD תכלת הרקיע לפני ה-30 במרץ, 2016, כדי להפעיל cmdlet AD PowerShell תכלת הרקיע הבאות כדי לאפשר התאמה רכים UPN עבור הארגון שלך בלבד:
  
 **ערכת-MsolDirSyncFeature-תכונה EnableSoftMatchOnUpn-אפשר $True**
  
התאמת רכים UPN מופעלת באופן אוטומטי עבור ארגונים שהפעילה לסנכרן AD תכלת הרקיע או לאחר 30 במרץ, 2016.
  
לקבלת מידע נוסף אודות הפיכת התאמה רכים UPN ותכונות אחרות של סינכרון, נא עיין [התחבר AD תכלת הרקיע התכונות של שירות הסינכרון](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

