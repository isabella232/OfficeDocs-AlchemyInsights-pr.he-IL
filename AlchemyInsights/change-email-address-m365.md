---
title: שנה כתובת דואר אלקטרוני של קבוצת Microsoft 365 או של Microsoft Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756558"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="20096-102">שנה כתובת דואר אלקטרוני של קבוצת Microsoft 365 או של Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="20096-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="20096-103">ניתן לשנות את כתובת הדואר האלקטרוני של קבוצת Microsoft 365 או של Microsoft Teams באמצעות [מרכז הניהול של Microsoft 365](https://admin.microsoft.com/). </span><span class="sxs-lookup"><span data-stu-id="20096-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="20096-104">כל שעליך לעשות הוא לבחור את הקבוצה ולבחור @עריכת כתובת דואר אלקטרוני.</span><span class="sxs-lookup"><span data-stu-id="20096-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="20096-105">תוכל גם להשתמש בפקודת EXO PowerShell הבאה כדי לשנות את כתובת ה- SMTP הראשית של קבוצת Microsoft 365 / ‏Microsoft Teams:</span><span class="sxs-lookup"><span data-stu-id="20096-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="20096-106">דוגמה:</span><span class="sxs-lookup"><span data-stu-id="20096-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
