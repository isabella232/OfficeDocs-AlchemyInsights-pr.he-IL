---
title: אין אפשרות לגשת לתיקיות ציבוריות
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341404"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>ל-Outlook אין אפשרות להתחבר לתיקיות ציבוריות

אם access public folder אינו עובד עבור חלק מהמשתמשים, נסה את הפעולות הבאות:

התחבר ל-קליפת PowerShell וקבע את התצורה של הפרמטר DefaultPublicFolderMailbox בחשבון המשתמש של הבעיה כדי להתאים לפרמטר בחשבון משתמש עובד.

דוגמה

קבלת-תיבת דואר WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

הגדרת תיבת דואר ProblemUser-DefaultPublicFolderMailbox \<value from previous command>

המתן שעה אחת לפחות כדי שהשינוי ייכנס לתוקף.

אם הבעיה נשארת, בצע [הליך זה](https://aka.ms/pfcte) כדי לפתור בעיות בגישה לתיקיות ציבוריות באמצעות Outlook.
 
**כדי לקבוע אילו משתמשים יוכלו לגשת לתיקיות ציבוריות באמצעות Outlook**:

1.  שימוש ב-Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true או $false  
      
    $true: אפשר למשתמשים לגשת לתיקיות ציבוריות ב-Outlook  
      
    $false: מנע גישת משתמשים לתיקיות ציבוריות ב-Outlook. (אפס) זהו ערך ברירת המחדל.  
        
2.  Set-OrganizationConfig-PublicFolderShowClientControl $true   
      
**הערה** הליך זה יכול לשלוט בחיבורים רק עם שולחן העבודה של Outlook עבור לקוחות Windows. משתמש יכול להמשיך לגשת לתיקיות ציבוריות באמצעות OWA או Outlook for Mac.
 
לקבלת מידע נוסף, ראה [הודעה על תמיכה בהתקשרויות מבוקרות לתיקיות ציבוריות ב-Outlook](https://aka.ms/controlpf).