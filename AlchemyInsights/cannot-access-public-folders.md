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
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996631"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook אין אפשרות להתחבר לתיקיות ציבוריות

אם הגישה לתיקיה ציבורית אינה פועלת עבור משתמשים מסוימים, נסה את הפעולות הבאות:

התחברות EXO PowerShell והגדר את הפרמטר DefaultPublicFolderMailbox בחשבון המשתמש הבעיה כך שיתאים לפרמטר בחשבון משתמש עובד.

דוגמה:

Get-Mailbox WorkingUser | ft DefaultציבוריFolderMailbox,EffectiveציבוריFolderMailbox

Set-Mailbox בעיהUser -DefaultציבוריFolderMailbox \<value from previous command>

המתן לפחות שעה אחת עד שהשינוי יתוקף.

אם הבעיה נשארת, בצע הליך [זה כדי לפתור](https://aka.ms/pfcte) בעיות גישה לתיקיה ציבורית באמצעות Outlook.
 
**כדי לקבוע אילו משתמשים יוכלו לגשת לתיקיות ציבוריות באמצעות Outlook**:

1.  השתמש <mailboxname> Set-CASMailbox-PublicFolderClientAccess $true או $false  
      
    $true: אפשר למשתמשים לגשת לתיקיות ציבוריות Outlook  
      
    $false: מניעת גישת משתמש לתיקיות ציבוריות ב- Outlook. (אפס) זהו ערך ברירת המחדל.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**הערה** הליך זה יכול לשלוט בחיבורים רק Outlook שולחן העבודה Windows לקוחות. משתמש יכול להמשיך לגשת לתיקיות ציבוריות באמצעות OWA או Outlook עבור Mac.
 
לקבלת מידע נוסף, ראה הודעה על תמיכה [עבור חיבורים מבוקרים לתיקיות ציבוריות ב- Outlook](https://aka.ms/controlpf).