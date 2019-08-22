---
title: המרת תיבת הדואר של המשתמש לתוך תיבת דואר משותפת?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496400"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a>המרה של תיבת הדואר של המשתמש לתוך תיבת דואר משותפת

באפשרותך להמיר תיבת הדואר של המשתמש לתיבת דואר משותפת רק אם למשתמש יש רשיון של Exchange. לאחר המרת הדואר, הוא ימשיך להופיע ברשימת משתמשים פעילים, מכיוון שהרשימה כוללת תיבות דואר משותפות. עם זאת, תיבת הדואר שהומרו גם תופיע ברשימה תיבת הדואר המשותפת. 
  
אם תנסה להמיר תיבת הדואר במסוף הניהול של Exchange ההמרה נכשלת, נקה את מטמון הדפדפן ואת קובצי ה-cookie ונסה שוב. אם הוא עדיין אינו עובד, נסה להמיר את תיבת הדואר של מעטפת ניהול Exchange על-ידי הפעלת הפקודה הבאה:
  
```
Set-Mailbox -Type Shared
```

מידע נוסף של המרת תיבת הדואר זמין [להמיר תיבת הדואר של המשתמש לתיבת דואר משותפת](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).
  
