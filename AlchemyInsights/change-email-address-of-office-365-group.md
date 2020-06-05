---
title: שינוי כתובת הדואר האלקטרוני של קבוצת מיקרוסופט 365
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
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580658"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="181c6-102">שינוי כתובת הדואר האלקטרוני של קבוצת מיקרוסופט 365</span><span class="sxs-lookup"><span data-stu-id="181c6-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="181c6-103">באפשרותך לשנות את כתובת הדואר האלקטרוני של קבוצת Microsoft 365 באמצעות מרכז הניהול.</span><span class="sxs-lookup"><span data-stu-id="181c6-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="181c6-104">פשוט בחר את הקבוצה ובחר את כתובת הדוא @edit.</span><span class="sxs-lookup"><span data-stu-id="181c6-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="181c6-105">באפשרותך גם להשתמש בעקבות הפקודה EXO PowerShell כדי לשנות את כתובת ה-SMTP הראשית של קבוצת Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="181c6-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="181c6-106">קבוצת מערכת-יוניסט <Group Name> -PrimarySmtpAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="181c6-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="181c6-107">דוגמה</span><span class="sxs-lookup"><span data-stu-id="181c6-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
