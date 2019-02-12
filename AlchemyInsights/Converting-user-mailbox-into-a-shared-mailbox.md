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
ms.openlocfilehash: 4da54121763fd33aa111f3bb3c26963cd271dc51
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906733"
---
באפשרותך להמיר תיבת הדואר של המשתמש לתיבת דואר משותפת רק אם למשתמש יש רשיון של Exchange. לאחר המרת הדואר, הוא ימשיך להופיע ברשימת משתמשים פעילים, מכיוון שהרשימה כוללת תיבות דואר משותפות. עם זאת, תיבת הדואר שהומרו גם תופיע ברשימה תיבת הדואר המשותפת. 
  
אם תנסה להמיר תיבת הדואר במסוף הניהול של Exchange ההמרה נכשלת, נקה את מטמון הדפדפן ואת קובצי ה-cookie ונסה שוב. אם הוא עדיין אינו עובד, נסה להמיר את תיבת הדואר של מעטפת ניהול Exchange על-ידי הפעלת הפקודה הבאה:
  
```
Set-Mailbox -Type Shared
```

מידע נוסף של המרת תיבת הדואר זמין [להמיר תיבת הדואר של המשתמש לתיבת דואר משותפת](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
