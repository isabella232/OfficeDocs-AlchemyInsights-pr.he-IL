---
title: אפשר ביקורת של תיבת דואר
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 81041685cf383a231a9a9739d6daffd6039b4602
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/22/2019
ms.locfileid: "30757819"
---
# <a name="enable-mailbox-auditing"></a>אפשר ביקורת של תיבת דואר

כדי להפעיל ביקורת על-ידי תיבת הדואר עבור משתמש בודד או ארגון שלם יש להפעיל את כלי cmdlet הבאים ממעטפת ההפעלה מרחוק:
  
 **משתמש יחיד**
  
Set-Mailbox - זהות "יורם חלון" - AuditEnabled $true
  
 **הארגון**
  
תיבת דואר-get - ResultSize מוגבל - סינון {"UserMailbox" RecipientTypeDetails - eq} | Set-Mailbox - AuditEnabled $true
  
[למד עוד](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

