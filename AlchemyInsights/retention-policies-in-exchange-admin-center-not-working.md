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
ms.openlocfilehash: 4d3ca121c8d22a0900f136f7f2a754dfb5b435f5
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522808"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="a9ff8-102">מדיניות שמירה במרכז הניהול של Exchange</span><span class="sxs-lookup"><span data-stu-id="a9ff8-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="a9ff8-103">אם אתה רוצה שנריץ בדיקות אוטומטיות עבור ההגדרות שהוזכרו להלן, בחר את לחצן החזרה _ Lt_--בראש דף זה ולאחר מכן הזן את כתובת הדואר האלקטרוני של המשתמש שיש לו בעיות עם מדיניות שמירה.</span><span class="sxs-lookup"><span data-stu-id="a9ff8-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="a9ff8-104">**בעיה:** מדיניות שמירה חדשה או מעודכנת במרכז הניהול של Exchange אינן חלות על תיבות דואר או פריטים אינם מועברים לתיבת הדואר של הארכיון או נמחקים.</span><span class="sxs-lookup"><span data-stu-id="a9ff8-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="a9ff8-105">**סיבות שורש:**</span><span class="sxs-lookup"><span data-stu-id="a9ff8-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="a9ff8-106">ייתכן שהסיבה לכך היא **שמסייע התיקיות המנוהל** לא עיבד את תיבת הדואר של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="a9ff8-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="a9ff8-107">מסייע התיקיות המנוהלות מנסה לעבד כל תיבת דואר בארגון המבוסס על ענן צמתים פעם בשבעה ימים.</span><span class="sxs-lookup"><span data-stu-id="a9ff8-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="a9ff8-108">אם אתה משנה תג שמירה או מחיל מדיניות שמירה שונה על תיבת דואר, באפשרותך להמתין עד לעיבוד תיבת הדואר, או להפעיל את המסייע של מסייע ההפעלה-cmdlet כדי להפעיל את מסייע התיקיות המנוהלות כדי לעבד תיבת דואר מסוימת.</span><span class="sxs-lookup"><span data-stu-id="a9ff8-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="a9ff8-109">הפעלת יישומון cmdlet זה שימושית לבדיקה או לפתרון בעיות של מדיניות שמירה או של הגדרות תג שמירה.</span><span class="sxs-lookup"><span data-stu-id="a9ff8-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="a9ff8-110">לקבלת מידע נוסף, בקר [הפעל את מסייע התיקיות המנוהלות](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="a9ff8-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="a9ff8-111">**פתרון הבעיה:** הפעל את הפקודה הבאה כדי להפעיל את מסייע התיקיות המנוהלות עבור תיבת דואר מסוימת:</span><span class="sxs-lookup"><span data-stu-id="a9ff8-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="a9ff8-112">הדבר עלול להתרחש גם אם **RetentionHold** **הופעלה** בתיבת הדואר.</span><span class="sxs-lookup"><span data-stu-id="a9ff8-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="a9ff8-113">אם תיבת הדואר הוצבה ב-RetentionHold, מדיניות השמירה בתיבת הדואר לא תעובד במהלך זמן זה.</span><span class="sxs-lookup"><span data-stu-id="a9ff8-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="a9ff8-114">לקבלת מפרטים נוספים על ההגדרה RetentionHold ראה: [החזקת שמירה של תיבת דואר](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="a9ff8-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="a9ff8-115">**פתרון**</span><span class="sxs-lookup"><span data-stu-id="a9ff8-115">**Solution:**</span></span>
    
  - <span data-ttu-id="a9ff8-116">בדוק את מצב ההגדרה RetentionHold בתיבת הדואר הספציפית ב- [Exo powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="a9ff8-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="a9ff8-117">הפעל את הפקודה הבאה כדי **להשבית** את RetentionHold בתיבת דואר מסוימת:</span><span class="sxs-lookup"><span data-stu-id="a9ff8-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="a9ff8-118">כעת, הפעל מחדש את מסייע התיקיות המנוהלות:</span><span class="sxs-lookup"><span data-stu-id="a9ff8-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="a9ff8-119">**הערה:** אם תיבת דואר קטנה מ-10 MB, מסייע התיקיות המנוהלות לא יעבד באופן אוטומטי את תיבת הדואר.</span><span class="sxs-lookup"><span data-stu-id="a9ff8-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="a9ff8-120">לקבלת מידע נוסף אודות מדיניות שמירה במרכז הניהול של Exchange, ראה:</span><span class="sxs-lookup"><span data-stu-id="a9ff8-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="a9ff8-121">תגיות שמירה ומדיניות שמירה</span><span class="sxs-lookup"><span data-stu-id="a9ff8-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="a9ff8-122">החלת מדיניות שמירה על תיבות דואר</span><span class="sxs-lookup"><span data-stu-id="a9ff8-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="a9ff8-123">הוספה או הסרה של תגי שמירה</span><span class="sxs-lookup"><span data-stu-id="a9ff8-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="a9ff8-124">כיצד לזהות את סוג החסימה שמוקמה בתיבת דואר</span><span class="sxs-lookup"><span data-stu-id="a9ff8-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
