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
ms.openlocfilehash: 2bcfb7cc174cd58b21e1bb0c82f0d7cdb25e2fdd
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506955"
---
# <a name="enable-mailbox-auditing"></a>הפיכת ביקורת תיבת דואר לזמינה

כדי להפעיל את ביקורת תיבת הדואר עבור משתמש יחיד או ארגון שלם, יש להפעיל את רכיבי ה-cmdlet הבאים ממעטפת החשמל המרוחקת:
  
 **משתמש יחיד**
  
הגדר-תיבת דואר-זהות "ג ' יין דאו"-מ$true השמע
  
 **ארגון**
  
קבל-תיבת דואר-ResultSize ללא הגבלה-מסנן {RecipientTypeDetails-eq "UserMailbox"} | הגדרת מ$true באמצעות תיבות דואר
  
[למד עוד](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

