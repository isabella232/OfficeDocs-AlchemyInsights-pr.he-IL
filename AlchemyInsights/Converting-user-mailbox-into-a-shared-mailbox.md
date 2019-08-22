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
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a><span data-ttu-id="83699-102">המרה של תיבת הדואר של המשתמש לתוך תיבת דואר משותפת</span><span class="sxs-lookup"><span data-stu-id="83699-102">Convert a user mail box into a shared mailbox</span></span>

<span data-ttu-id="83699-103">באפשרותך להמיר תיבת הדואר של המשתמש לתיבת דואר משותפת רק אם למשתמש יש רשיון של Exchange.</span><span class="sxs-lookup"><span data-stu-id="83699-103">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="83699-104">לאחר המרת הדואר, הוא ימשיך להופיע ברשימת משתמשים פעילים, מכיוון שהרשימה כוללת תיבות דואר משותפות.</span><span class="sxs-lookup"><span data-stu-id="83699-104">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="83699-105">עם זאת, תיבת הדואר שהומרו גם תופיע ברשימה תיבת הדואר המשותפת.</span><span class="sxs-lookup"><span data-stu-id="83699-105">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="83699-106">אם תנסה להמיר תיבת הדואר במסוף הניהול של Exchange ההמרה נכשלת, נקה את מטמון הדפדפן ואת קובצי ה-cookie ונסה שוב.</span><span class="sxs-lookup"><span data-stu-id="83699-106">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="83699-107">אם הוא עדיין אינו עובד, נסה להמיר את תיבת הדואר של מעטפת ניהול Exchange על-ידי הפעלת הפקודה הבאה:</span><span class="sxs-lookup"><span data-stu-id="83699-107">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="83699-108">מידע נוסף של המרת תיבת הדואר זמין [להמיר תיבת הדואר של המשתמש לתיבת דואר משותפת](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span><span class="sxs-lookup"><span data-stu-id="83699-108">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span></span>
  
