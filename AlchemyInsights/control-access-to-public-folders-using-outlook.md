---
title: שליטה בגישה לתיקיות ציבוריות באמצעות Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816741"
---
# <a name="control-access-to-public-folders-using-outlook"></a>שליטה בגישה לתיקיות ציבוריות באמצעות Outlook

כדי לקבוע אילו משתמשים יוכלו לגשת לתיקיות ציבוריות באמצעות Outlook:

1. השתמש ב- `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: אפשר למשתמשים לגשת לתיקיות ציבוריות ב- Outlook  
$false: מניעת גישת משתמש לתיקיות ציבוריות ב- Outlook. (אפס) זהו ערך ברירת המחדל.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

הערה: הליך זה יכול לשלוט רק בחיבורים עם שולחן העבודה של Outlook עבור לקוחות Windows. המשתמשים יכולים להמשיך לגשת לתיקיות ציבוריות באמצעות OWA או Outlook עבור Mac.

לקבלת מידע נוסף, ראה [חיבורים מבוקרים לתיקיות ציבוריות ב- Outlook](https://aka.ms/controlpf) לקבלת מידע נוסף.
