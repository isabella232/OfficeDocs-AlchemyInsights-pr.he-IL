---
title: הפיכת ביקורת תיבת דואר לזמינה
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: ae11d6be0789a5662d202b85268480a3d42922c4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703572"
---
# <a name="enable-mailbox-auditing"></a>הפיכת ביקורת תיבת דואר לזמינה

כדי להפעיל את ביקורת תיבת הדואר עבור משתמש יחיד או ארגון שלם, יש להפעיל את רכיבי ה-cmdlet הבאים ממעטפת החשמל המרוחקת:
  
 **משתמש יחיד**
  
הגדר-תיבת דואר-זהות "ג ' יין דאו"-מ$true השמע
  
 **ארגון**
  
קבל-תיבת דואר-ResultSize ללא הגבלה-מסנן {RecipientTypeDetails-eq "UserMailbox"} | הגדרת מ$true באמצעות תיבות דואר
  
[למד עוד](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

