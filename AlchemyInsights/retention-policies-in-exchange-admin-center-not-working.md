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
ms.openlocfilehash: e2fb22f872be0eefc3b4b78b18cd09baffa66cda
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742434"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="67854-102">מדיניות שמירה במרכז הניהול של Exchange</span><span class="sxs-lookup"><span data-stu-id="67854-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="67854-103">**בעיה:** מדיניות שמירה חדשה או מעודכנת במרכז הניהול של Exchange אינן חלות על תיבות דואר או פריטים אינם מועברים לתיבת הדואר של הארכיון או נמחקים.</span><span class="sxs-lookup"><span data-stu-id="67854-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="67854-104">**סיבות שורש:**</span><span class="sxs-lookup"><span data-stu-id="67854-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="67854-105">ייתכן שהסיבה לכך היא **שמסייע התיקיות המנוהל** לא עיבד את תיבת הדואר של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="67854-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="67854-106">מסייע התיקיות המנוהלות מנסה לעבד כל תיבת דואר בארגון המבוסס על ענן צמתים פעם בשבעה ימים.</span><span class="sxs-lookup"><span data-stu-id="67854-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="67854-107">אם אתה משנה תג שמירה או מחיל מדיניות שמירה שונה על תיבת דואר, באפשרותך להמתין עד לעיבוד תיבת הדואר, או להפעיל את המסייע של מסייע ההפעלה-cmdlet כדי להפעיל את מסייע התיקיות המנוהלות כדי לעבד תיבת דואר מסוימת.</span><span class="sxs-lookup"><span data-stu-id="67854-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="67854-108">הפעלת יישומון cmdlet זה שימושית לבדיקה או לפתרון בעיות של מדיניות שמירה או של הגדרות תג שמירה.</span><span class="sxs-lookup"><span data-stu-id="67854-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="67854-109">לקבלת מידע נוסף, בקר [הפעל את מסייע התיקיות המנוהלות](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="67854-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="67854-110">**פתרון הבעיה:** הפעל את הפקודה הבאה כדי להפעיל את מסייע התיקיות המנוהלות עבור תיבת דואר מסוימת:</span><span class="sxs-lookup"><span data-stu-id="67854-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="67854-111">הדבר עלול להתרחש גם אם **RetentionHold** **הופעלה** בתיבת הדואר.</span><span class="sxs-lookup"><span data-stu-id="67854-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="67854-112">אם תיבת הדואר הוצבה ב-RetentionHold, מדיניות השמירה בתיבת הדואר לא תעובד במהלך זמן זה.</span><span class="sxs-lookup"><span data-stu-id="67854-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="67854-113">לקבלת מפרטים נוספים על ההגדרה RetentionHold ראה: [החזקת שמירה של תיבת דואר](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="67854-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="67854-114">**פתרון**</span><span class="sxs-lookup"><span data-stu-id="67854-114">**Solution:**</span></span>
    
  - <span data-ttu-id="67854-115">בדוק את מצב ההגדרה RetentionHold בתיבת הדואר הספציפית ב- [Exo powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="67854-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="67854-116">הפעל את הפקודה הבאה כדי **להשבית** את RetentionHold בתיבת דואר מסוימת:</span><span class="sxs-lookup"><span data-stu-id="67854-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="67854-117">כעת, הפעל מחדש את מסייע התיקיות המנוהלות:</span><span class="sxs-lookup"><span data-stu-id="67854-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="67854-118">**הערה:** אם תיבת דואר קטנה מ-10 MB, מסייע התיקיות המנוהלות לא יעבד באופן אוטומטי את תיבת הדואר.</span><span class="sxs-lookup"><span data-stu-id="67854-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="67854-119">לקבלת מידע נוסף אודות מדיניות שמירה במרכז הניהול של Exchange, ראה:</span><span class="sxs-lookup"><span data-stu-id="67854-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="67854-120">תגיות שמירה ומדיניות שמירה</span><span class="sxs-lookup"><span data-stu-id="67854-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="67854-121">החלת מדיניות שמירה על תיבות דואר</span><span class="sxs-lookup"><span data-stu-id="67854-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="67854-122">הוספה או הסרה של תגי שמירה</span><span class="sxs-lookup"><span data-stu-id="67854-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="67854-123">כיצד לזהות את סוג החסימה שמוקמה בתיבת דואר</span><span class="sxs-lookup"><span data-stu-id="67854-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
