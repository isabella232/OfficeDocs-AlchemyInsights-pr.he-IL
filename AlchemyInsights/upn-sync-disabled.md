---
title: סינכרון UPN זמין
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: f390d659b191fa4c44bd7c8acb32409cd3021489
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36532332"
---
# <a name="upn-sync-disabled"></a>סינכרון UPN זמין

אם התחלת סינכרון AD תכלת הרקיע לפני ה-30 במרץ, 2016, כדי להפעיל cmdlet AD PowerShell תכלת הרקיע הבאות כדי לאפשר התאמה רכים UPN עבור הארגון שלך בלבד:
  
 **ערכת-MsolDirSyncFeature-תכונה EnableSoftMatchOnUpn-אפשר $True**
  
התאמת רכים UPN מופעלת באופן אוטומטי עבור ארגונים שהפעילה לסנכרן AD תכלת הרקיע או לאחר 30 במרץ, 2016.
  
לקבלת מידע נוסף אודות הפיכת התאמה רכים UPN ותכונות אחרות של סינכרון, נא עיין [התחבר AD תכלת הרקיע התכונות של שירות הסינכרון](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

