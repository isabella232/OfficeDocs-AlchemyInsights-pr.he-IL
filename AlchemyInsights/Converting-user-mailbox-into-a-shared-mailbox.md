---
title: המרת תיבת הדואר של המשתמש לתוך תיבת דואר משותפת?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Priority
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 22ad1b3fb818b40bcd77974031735f931e986968
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29472130"
---
באפשרותך להמיר תיבת הדואר של המשתמש לתיבת דואר משותפת רק אם למשתמש יש רשיון של Exchange. לאחר המרת הדואר, הוא ימשיך להופיע ברשימת משתמשים פעילים, מכיוון שהרשימה כוללת תיבות דואר משותפות. עם זאת, תיבת הדואר שהומרו גם תופיע ברשימה תיבת הדואר המשותפת. 
  
אם תנסה להמיר תיבת הדואר במסוף הניהול של Exchange ההמרה נכשלת, נקה את מטמון הדפדפן ואת קובצי ה-cookie ונסה שוב. אם הוא עדיין אינו עובד, נסה להמיר את תיבת הדואר של מעטפת ניהול Exchange על-ידי הפעלת הפקודה הבאה:
  
```
Set-Mailbox -Type Shared
```

מידע נוסף של המרת תיבת הדואר זמין [להמיר תיבת הדואר של המשתמש לתיבת דואר משותפת](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
