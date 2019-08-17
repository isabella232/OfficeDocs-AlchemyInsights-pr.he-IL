---
title: מדיניות שמירה במרכז הניהול של Exchange אינו פועל
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: d0af4c933f262fe1ec4c2a6ff16d5f6195398b0d
ms.sourcegitcommit: e98443a049108e0dc83d63895af66944bdb1f108
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/16/2019
ms.locfileid: "36444809"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="998c9-102">מדיניות שמירה במרכז הניהול של Exchange</span><span class="sxs-lookup"><span data-stu-id="998c9-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="998c9-103">**בעיה:** חדשות שנוצרו או לא ניתן להחיל מדיניות שמירה מעודכן במרכז הניהול של Exchange אל תיבות דואר או פריטים לא מועבר לתיבת הדואר ארכיון או נמחקה.</span><span class="sxs-lookup"><span data-stu-id="998c9-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="998c9-104">**סיבות בסיס:**</span><span class="sxs-lookup"><span data-stu-id="998c9-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="998c9-105">ייתכן שהדבר נובע מכך **מסייע התיקיות המנוהלות** לא עיבד הדואר של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="998c9-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="998c9-106">מנוהל מסייע התיקיות מנסה לעבד כל הדואר בארגון שלך המבוסס על ענן פעם אחת כל שבעה ימים.</span><span class="sxs-lookup"><span data-stu-id="998c9-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="998c9-107">אם תשנה תגית שמירה או להחיל מדיניות שמירה שונה לתיבת דואר, באפשרותך להמתין עד מנוהל תיקיה לסייע מעבדת את תיבת הדואר, או שבאפשרותך להפעיל cmdlet Start-ManagedFolderAssistant כדי להפעיל את ניהול מסייע התיקיות לעיבוד ספציפי תיבת הדואר.</span><span class="sxs-lookup"><span data-stu-id="998c9-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="998c9-108">הפעלת cmdlet זה שימושי עבור בדיקה או פתרון בעיות מדיניות שמירה או הגדרות תגית שמירה.</span><span class="sxs-lookup"><span data-stu-id="998c9-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="998c9-109">לקבלת מידע נוסף, בקר [להפעיל את מנוהל מסייע התיקיות](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="998c9-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="998c9-110">**פתרון:** הפעל את הפקודה הבאה כדי להתחיל את מנוהל מסייע התיקיות עבור תיבת דואר מסוימת:</span><span class="sxs-lookup"><span data-stu-id="998c9-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="998c9-111">הדבר עלול להיות להתרחש גם אם **RetentionHold** הפך **לזמין** בתיבת הדואר.</span><span class="sxs-lookup"><span data-stu-id="998c9-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="998c9-112">אם תיבת הדואר הוצב על RetentionHold, מדיניות השמירה בתיבת הדואר לא יעובדו במהלך זמן זה.</span><span class="sxs-lookup"><span data-stu-id="998c9-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="998c9-113">עבור informaton נוסף על ראה הגדרה RetentionHold: [החזק השמירה של תיבת הדואר](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="998c9-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="998c9-114">**פתרון:**</span><span class="sxs-lookup"><span data-stu-id="998c9-114">**Solution:**</span></span>
    
  - <span data-ttu-id="998c9-115">בדוק את המצב של הגדרת RetentionHold בתיבת הדואר ספציפי ב- [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="998c9-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="998c9-116">הפעל את הפקודה הבאה כדי **להשבית** RetentionHold תיבת דואר מסוימת:</span><span class="sxs-lookup"><span data-stu-id="998c9-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="998c9-117">כעת, הפעל מחדש את התיקיה מנוהל המסייע:</span><span class="sxs-lookup"><span data-stu-id="998c9-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="998c9-118">**הערה:** אם תיבת דואר קטן מ- 10 MB, מנוהל מסייע התיקיות לא יעבד באופן אוטומטי את תיבת הדואר.</span><span class="sxs-lookup"><span data-stu-id="998c9-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="998c9-119">לקבלת מידע נוסף אודות מדיניות השמירה במרכז הניהול של Exchange, ראה:</span><span class="sxs-lookup"><span data-stu-id="998c9-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="998c9-120">תגיות השמירה ובמדיניות שמירת</span><span class="sxs-lookup"><span data-stu-id="998c9-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="998c9-121">החל מדיניות שמירה על תיבות דואר</span><span class="sxs-lookup"><span data-stu-id="998c9-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="998c9-122">הוספה או הסרה של תגיות שמירה</span><span class="sxs-lookup"><span data-stu-id="998c9-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="998c9-123">כיצד לזהות את סוג החסימה מוצבים תיבת דואר</span><span class="sxs-lookup"><span data-stu-id="998c9-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/en-us/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
