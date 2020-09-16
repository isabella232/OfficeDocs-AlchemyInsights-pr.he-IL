---
title: הפיכת ביקורת תיבת דואר לזמינה
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
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 404ef9ecd824541f98471bb8797f5f6e025012b7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806292"
---
# <a name="enable-mailbox-auditing"></a>הפיכת ביקורת תיבת דואר לזמינה

כדי להפוך ביקורת של תיבות דואר לזמינה עבור משתמש בודד או של ארגון שלם, יש להפעיל את רכיבי ה-cmdlet הבאים מתוך מעטפת Power מרוחקת:
  
 **משתמש בודד**
  
Set-תיבת דואר-זהות "ג'יין דאו"-AuditEnabled $true
  
 **ארגון**
  
Get-Mailbox-ResultSize ללא הגבלה-מסנן {RecipientTypeDetails-eq "UserMailbox"} | Set-AuditEnabled $true
  
[למד עוד](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

