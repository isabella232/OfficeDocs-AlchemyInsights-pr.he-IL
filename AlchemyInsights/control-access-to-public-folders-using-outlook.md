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
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032559"
---
# <a name="control-access-to-public-folders-using-outlook"></a>שליטה בגישה לתיקיות ציבוריות באמצעות Outlook

כדי לקבוע אילו משתמשים יוכלו לגשת לתיקיות ציבוריות באמצעות Outlook:

1. השתמש ב- `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: אפשר למשתמשים לגשת לתיקיות ציבוריות Outlook  
$false: מניעת גישת משתמש לתיקיות ציבוריות ב- Outlook. (אפס) זהו ערך ברירת המחדל.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

הערה: הליך זה יכול לשלוט רק בחיבורים Outlook שולחן העבודה עבור Windows לקוחות. המשתמשים יכולים להמשיך לגשת לתיקיות ציבוריות באמצעות OWA או Outlook עבור Mac.

לקבלת מידע נוסף, ראה [חיבורים מבוקרים לתיקיות ציבוריות ב- Outlook](https://aka.ms/controlpf) לקבלת מידע נוסף.
