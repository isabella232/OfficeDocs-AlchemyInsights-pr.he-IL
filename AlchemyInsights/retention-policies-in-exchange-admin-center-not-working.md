---
title: מדיניות שמירה במרכז ניהול של Exchange אינה פועלת
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 3040365b9d686bcbcce60977ee9bdbbaffc70b24
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502608"
---
# <a name="retention-policies-in-exchange-admin-center"></a>מדיניות שמירה במרכז הניהול של Exchange

 **בעיה:** מדיניות שמירה חדשה או מעודכנת במרכז הניהול של Exchange אינן חלות על תיבות דואר או פריטים אינם מועברים לתיבת הדואר של הארכיון או נמחקים. 
  
 **סיבות שורש:**
  
- ייתכן שהסיבה לכך היא **שמסייע התיקיות המנוהל** לא עיבד את תיבת הדואר של המשתמש. מסייע התיקיות המנוהלות מנסה לעבד כל תיבת דואר בארגון המבוסס על ענן צמתים פעם בשבעה ימים. אם אתה משנה תג שמירה או מחיל מדיניות שמירה שונה על תיבת דואר, באפשרותך להמתין עד לעיבוד תיבת הדואר, או להפעיל את המסייע של מסייע ההפעלה-cmdlet כדי להפעיל את מסייע התיקיות המנוהלות כדי לעבד תיבת דואר מסוימת. הפעלת יישומון cmdlet זה שימושית לבדיקה או לפתרון בעיות של מדיניות שמירה או של הגדרות תג שמירה. לקבלת מידע נוסף, בקר [הפעל את מסייע התיקיות המנוהלות](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **פתרון הבעיה:** הפעל את הפקודה הבאה כדי להפעיל את מסייע התיקיות המנוהלות עבור תיבת דואר מסוימת:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- הדבר עלול להתרחש גם אם **RetentionHold** **הופעלה** בתיבת הדואר. אם תיבת הדואר הוצבה ב-RetentionHold, מדיניות השמירה בתיבת הדואר לא תעובד במהלך זמן זה. לקבלת מפרטים נוספים על ההגדרה RetentionHold ראה: [החזקת שמירה של תיבת דואר](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **פתרון**
    
  - בדוק את מצב ההגדרה RetentionHold בתיבת הדואר הספציפית ב- [Exo powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - הפעל את הפקודה הבאה כדי **להשבית** את RetentionHold בתיבת דואר מסוימת:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - כעת, הפעל מחדש את מסייע התיקיות המנוהלות:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **הערה:** אם תיבת דואר קטנה מ-10 MB, מסייע התיקיות המנוהלות לא יעבד באופן אוטומטי את תיבת הדואר.
 
לקבלת מידע נוסף אודות מדיניות שמירה במרכז הניהול של Exchange, ראה:
- [תגיות שמירה ומדיניות שמירה](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [החלת מדיניות שמירה על תיבות דואר](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [הוספה או הסרה של תגי שמירה](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [כיצד לזהות את סוג החסימה שמוקמה בתיבת דואר](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
