---
title: שינוי כתובת הדואר האלקטרוני של קבוצת Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/27/2020
ms.locfileid: "44282923"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a><span data-ttu-id="c77a7-102">שינוי כתובת הדואר האלקטרוני של קבוצת Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c77a7-102">Change email address of an Microsoft 365 group</span></span>

<span data-ttu-id="c77a7-103">באפשרותך לשנות את כתובת הדואר האלקטרוני של קבוצת Microsoft 365 באמצעות מרכז הניהול.</span><span class="sxs-lookup"><span data-stu-id="c77a7-103">You can change the email address of an Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="c77a7-104">פשוט בחר את הקבוצה ובחר את כתובת הדוא @edit.</span><span class="sxs-lookup"><span data-stu-id="c77a7-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="c77a7-105">באפשרותך גם להשתמש בעקבות הפקודה EXO PowerShell כדי לשנות את כתובת ה-SMTP הראשית של קבוצת Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="c77a7-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Microsoft 365 group:</span></span>

<span data-ttu-id="c77a7-106">קבוצת מערכת-יוניסט <Group Name> -PrimarySmtpAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="c77a7-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="c77a7-107">דוגמה</span><span class="sxs-lookup"><span data-stu-id="c77a7-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
