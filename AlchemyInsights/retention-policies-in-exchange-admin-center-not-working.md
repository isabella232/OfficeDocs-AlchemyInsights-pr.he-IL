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
 <span data-ttu-id="6b54f-102">**בעיה:** חדשות שנוצרו או לא ניתן להחיל מדיניות שמירה מעודכן במרכז הניהול של Exchange אל תיבות דואר או פריטים לא מועבר לתיבת הדואר ארכיון או נמחקה.</span><span class="sxs-lookup"><span data-stu-id="6b54f-102">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="6b54f-103">**סיבות בסיס:**</span><span class="sxs-lookup"><span data-stu-id="6b54f-103">**Root Causes:**</span></span>
  
- <span data-ttu-id="6b54f-p101">ייתכן שהדבר נובע מכך **מסייע התיקיות המנוהלות** לא עיבד הדואר של המשתמש. מנוהל מסייע התיקיות מנסה לעבד כל הדואר בארגון שלך המבוסס על ענן פעם אחת כל שבעה ימים. אם תשנה תגית שמירה או להחיל מדיניות שמירה שונה לתיבת דואר, באפשרותך להמתין עד מנוהל תיקיה לסייע מעבדת את תיבת הדואר, או שבאפשרותך להפעיל cmdlet Start-ManagedFolderAssistant כדי להפעיל את ניהול מסייע התיקיות לעיבוד ספציפי תיבת הדואר. הפעלת cmdlet זה שימושי עבור בדיקה או פתרון בעיות מדיניות שמירה או הגדרות תגית שמירה. לקבלת מידע נוסף, בקר [להפעיל את מנוהל מסייע התיקיות](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="6b54f-p101">This may be because the **Managed Folder Assistant** has not processed the user's mailbox. The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days. If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox. Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings. For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="6b54f-109">**פתרון:** הפעל את הפקודה הבאה כדי להתחיל את מנוהל מסייע התיקיות עבור תיבת דואר מסוימת:</span><span class="sxs-lookup"><span data-stu-id="6b54f-109">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="6b54f-p102">הדבר עלול להיות להתרחש גם אם **RetentionHold** הפך **לזמין** בתיבת הדואר. אם תיבת הדואר הוצב על RetentionHold, מדיניות השמירה בתיבת הדואר לא יעובדו במהלך זמן זה. עבור informaton נוסף על ראה הגדרה RetentionHold: [החזק השמירה של תיבת הדואר](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="6b54f-p102">This may also be occur if **RetentionHold** has been **enabled** on the mailbox. If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time. For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="6b54f-113">פתרון</span><span class="sxs-lookup"><span data-stu-id="6b54f-113">**Solution:**</span></span>
    
  - <span data-ttu-id="6b54f-114">בדוק את המצב של הגדרת RetentionHold בתיבת הדואר ספציפי ב- [EXO powershell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="6b54f-114">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="6b54f-115">הפעל את הפקודה הבאה כדי **להשבית** RetentionHold תיבת דואר מסוימת:</span><span class="sxs-lookup"><span data-stu-id="6b54f-115">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="6b54f-116">כעת, הפעל מחדש את התיקיה מנוהל המסייע:</span><span class="sxs-lookup"><span data-stu-id="6b54f-116">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="6b54f-117">**הערה:** אם תיבת דואר קטן מ- 10 MB, מנוהל מסייע התיקיות לא יעבד באופן אוטומטי את תיבת הדואר.</span><span class="sxs-lookup"><span data-stu-id="6b54f-117">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

