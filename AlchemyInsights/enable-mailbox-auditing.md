---
title: אפשר ביקורת של תיבת דואר
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: bd94ec10f9df2e72ec6e3d8552d2eb80212a9d78
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28291707"
---
# <a name="enable-mailbox-auditing"></a>אפשר ביקורת של תיבת דואר

כדי להפעיל ביקורת על-ידי תיבת הדואר עבור משתמש בודד או ארגון שלם יש להפעיל את כלי cmdlet הבאים ממעטפת ההפעלה מרחוק:
  
 **משתמש יחיד**
  
Set-Mailbox - זהות "יורם חלון" - AuditEnabled $true
  
 **הארגון**
  
תיבת דואר-get - ResultSize מוגבל - סינון {"UserMailbox" RecipientTypeDetails - eq} | Set-Mailbox - AuditEnabled $true
  
[מידע נוסף](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

