---
title: סינכרון UPN אינו זמין
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749515"
---
# <a name="upn-sync-disabled"></a>סינכרון UPN אינו זמין

אם התחלת לסנכרן את התכלת לספירה לפני 30 במרץ, 2016, הפעל את ה-cmdlet הבאים של תכלת לספירה כדי להפוך התאמה רכה של UPN לזמינה עבור הארגון שלך בלבד:
  
 **Set-MsolDirSyncFeature-EnableSoftMatchOnUpn-הפיכת התכונה לזמינה $True**
  
התאמה רכה של UPN מופעלת באופן אוטומטי עבור ארגונים שהתחילו לסנכרן את התכלת לספירה ב-30 במרץ או אחרי ה-30 במרץ 2016.
  
לקבלת מידע נוסף על הפעלת התאמה רכה ב-UPN ובתכונות סינכרון אחרות, ראה [התכונה תכלת AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

