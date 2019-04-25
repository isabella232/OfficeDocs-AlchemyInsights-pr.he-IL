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
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32374324"
---
<span data-ttu-id="e76ec-102">באפשרותך להמיר תיבת הדואר של המשתמש לתיבת דואר משותפת רק אם למשתמש יש רשיון של Exchange.</span><span class="sxs-lookup"><span data-stu-id="e76ec-102">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="e76ec-103">לאחר המרת הדואר, הוא ימשיך להופיע ברשימת משתמשים פעילים, מכיוון שהרשימה כוללת תיבות דואר משותפות.</span><span class="sxs-lookup"><span data-stu-id="e76ec-103">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="e76ec-104">עם זאת, תיבת הדואר שהומרו גם תופיע ברשימה תיבת הדואר המשותפת.</span><span class="sxs-lookup"><span data-stu-id="e76ec-104">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="e76ec-105">אם תנסה להמיר תיבת הדואר במסוף הניהול של Exchange ההמרה נכשלת, נקה את מטמון הדפדפן ואת קובצי ה-cookie ונסה שוב.</span><span class="sxs-lookup"><span data-stu-id="e76ec-105">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="e76ec-106">אם הוא עדיין אינו עובד, נסה להמיר את תיבת הדואר של מעטפת ניהול Exchange על-ידי הפעלת הפקודה הבאה:</span><span class="sxs-lookup"><span data-stu-id="e76ec-106">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="e76ec-107">מידע נוסף של המרת תיבת הדואר זמין [להמיר תיבת הדואר של המשתמש לתיבת דואר משותפת](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span><span class="sxs-lookup"><span data-stu-id="e76ec-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
