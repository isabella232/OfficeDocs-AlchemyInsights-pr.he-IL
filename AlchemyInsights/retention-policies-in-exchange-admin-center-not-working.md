---
title: מדיניות שמירה במרכז הניהול של Exchange אינו פועל
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 0ceb1737040f0304bfe8b611241ce1deef487652
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29472631"
---
 **בעיה:** חדשות שנוצרו או לא ניתן להחיל מדיניות שמירה מעודכן במרכז הניהול של Exchange אל תיבות דואר או פריטים לא מועבר לתיבת הדואר ארכיון או נמחקה. 
  
 **סיבות בסיס:**
  
- ייתכן שהדבר נובע מכך **מסייע התיקיות המנוהלות** לא עיבד הדואר של המשתמש. מנוהל מסייע התיקיות מנסה לעבד כל הדואר בארגון שלך המבוסס על ענן פעם אחת כל שבעה ימים. אם תשנה תגית שמירה או להחיל מדיניות שמירה שונה לתיבת דואר, באפשרותך להמתין עד מנוהל תיקיה לסייע מעבדת את תיבת הדואר, או שבאפשרותך להפעיל cmdlet Start-ManagedFolderAssistant כדי להפעיל את ניהול מסייע התיקיות לעיבוד ספציפי תיבת הדואר. הפעלת cmdlet זה שימושי עבור בדיקה או פתרון בעיות מדיניות שמירה או הגדרות תגית שמירה. לקבלת מידע נוסף, בקר [להפעיל את מנוהל מסייע התיקיות](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **פתרון:** הפעל את הפקודה הבאה כדי להתחיל את מנוהל מסייע התיקיות עבור תיבת דואר מסוימת: 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- הדבר עלול להיות להתרחש גם אם **RetentionHold** הפך **לזמין** בתיבת הדואר. אם תיבת הדואר הוצב על RetentionHold, מדיניות השמירה בתיבת הדואר לא יעובדו במהלך זמן זה. עבור informaton נוסף על ראה הגדרה RetentionHold: [החזק השמירה של תיבת הדואר](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    פתרון
    
  - בדוק את המצב של הגדרת RetentionHold בתיבת הדואר ספציפי ב- [EXO powershell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - הפעל את הפקודה הבאה כדי **להשבית** RetentionHold תיבת דואר מסוימת: 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - כעת, הפעל מחדש את התיקיה מנוהל המסייע:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **הערה:** אם תיבת דואר קטן מ- 10 MB, מנוהל מסייע התיקיות לא יעבד באופן אוטומטי את תיבת הדואר. 
  

