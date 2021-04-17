---
title: אין אפשרות לגשת לתיקיות ציבוריות
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819513"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>ל- Outlook אין אפשרות להתחבר לתיקיות ציבוריות

אם הגישה לתיקיה ציבורית אינה פועלת עבור משתמשים מסוימים, נסה את הפעולות הבאות:

התחבר ל- EXO PowerShell והגדר את הפרמטר DefaultPublicFolderMailbox בחשבון המשתמש הלבעיה כך שיתאים לפרמטר בחשבון משתמש פועל.

דוגמה:

Get-Mailbox WorkingUser | ft DefaultציבוריFolderMailbox,EffectiveציבוריFolderMailbox

Set-Mailbox בעיהUser -DefaultציבוריFolderMailbox \<value from previous command>

המתן לפחות שעה אחת עד שהשינוי יתוקף.

אם הבעיה נשארת, בצע הליך זה [כדי לפתור](https://aka.ms/pfcte) בעיות גישה לתיקיה ציבורית באמצעות Outlook.
 
**כדי לקבוע אילו משתמשים יוכלו לגשת לתיקיות ציבוריות באמצעות Outlook**:

1.  השתמש <mailboxname> Set-CASMailbox-PublicFolderClientAccess $true או $false  
      
    $true: אפשר למשתמשים לגשת לתיקיות ציבוריות ב- Outlook  
      
    $false: מניעת גישת משתמש לתיקיות ציבוריות ב- Outlook. (אפס) זהו ערך ברירת המחדל.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**הערה** הליך זה יכול לשלוט בחיבורים רק עם שולחן העבודה של Outlook עבור לקוחות Windows. משתמש יכול להמשיך לגשת לתיקיות ציבוריות באמצעות OWA או Outlook עבור Mac.
 
לקבלת מידע נוסף, ראה [הודעה על תמיכה עבור חיבורים מבוקרים לתיקיות ציבוריות ב- Outlook](https://aka.ms/controlpf).