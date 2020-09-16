---
title: מדיניות שמירה במרכז הניהול של Exchange אינה פועלת
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740511"
---
# <a name="retention-policies-in-exchange-admin-center"></a>מדיניות שמירה במרכז הניהול של Exchange

אם ברצונך לבצע בדיקות אוטומטיות עבור ההגדרות המוזכרות להלן, בחר את לחצן ' הקודם ' < '-בחלק העליון של דף זה, ולאחר מכן הזן את כתובת הדואר האלקטרוני של המשתמש שנתקל בבעיות עם מדיניות שמירה.

 **בעיה:** מדיניות שמירה חדשה שנוצרה או עודכנה במרכז הניהול של Exchange אינה חלה על תיבות דואר או פריטים אינם מועברים לתיבת הדואר של הארכיון או נמחקים. 
  
 **גורמים בסיסיים:**
  
- ייתכן שהסיבה לכך היא **שמסייע התיקיות המנוהלות** לא עיבד את תיבת הדואר של המשתמש. מסייע התיקיות המנוהלות מנסה לעבד כל תיבת דואר בארגון מבוסס הענן שלך פעם בכל שבעה ימים. אם אתה משנה תגית שמירה או מחיל מדיניות שמירה שונה על תיבת דואר, באפשרותך להמתין עד לקבלת סיוע בתיקיה המנוהלת לעיבוד תיבת הדואר, או להפעיל את ה-cmdlet Start-ManagedFolderAssistant כדי להפעיל את מסייע התיקיות המנוהלות כדי לעבד תיבת דואר ספציפית. הפעלת cmdlet זה שימושית לבדיקה או לפתרון בעיות של מדיניות שמירה או הגדרות של תגית שמירה. לקבלת מידע נוסף, בקר [בהפעלת מסייע התיקיות המנוהלות](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **הפתרון:** הפעל את הפקודה הבאה כדי להפעיל את מסייע התיקיות המנוהלות עבור תיבת דואר ספציפית:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- הדבר עשוי להתרחש גם אם **RetentionHold** הפך **לזמין** בתיבת הדואר. אם תיבת הדואר ממוקמת ב-RetentionHold, מדיניות השמירה בתיבת הדואר לא תעובד במהלך זמן זה. לקבלת מידע נוסף על informaton בהגדרה RetentionHold ראה: [החזקת שמירה של תיבת דואר](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **פתרון**
    
  - בדוק את מצב ההגדרה RetentionHold בתיבת הדואר הספציפית ב- [קליפת powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - הפעל את הפקודה הבאה כדי **להפוך את RetentionHold ללא זמין** בתיבת דואר ספציפית:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - כעת, הפעל מחדש את מסייע התיקיות המנוהלות:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **הערה:** אם תיבת דואר קטנה מ-10 MB, מסייע התיקיות המנוהלות לא יעבד באופן אוטומטי את תיבת הדואר.
 
לקבלת מידע נוסף אודות מדיניות שמירה במרכז הניהול של Exchange, ראה:
- [תגי שמירה ומדיניות שמירה](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [החלת מדיניות שמירה על תיבות דואר](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [הוספה או הסרה של תגי שמירה](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [כיצד לזהות את סוג החסימה שתמוקם בתיבת דואר](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
