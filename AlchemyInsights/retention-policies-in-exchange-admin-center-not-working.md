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
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="215db-102">מדיניות שמירה במרכז הניהול של Exchange</span><span class="sxs-lookup"><span data-stu-id="215db-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="215db-103">אם ברצונך לבצע בדיקות אוטומטיות עבור ההגדרות המוזכרות להלן, בחר את לחצן ' הקודם ' < '-בחלק העליון של דף זה, ולאחר מכן הזן את כתובת הדואר האלקטרוני של המשתמש שנתקל בבעיות עם מדיניות שמירה.</span><span class="sxs-lookup"><span data-stu-id="215db-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="215db-104">**בעיה:** מדיניות שמירה חדשה שנוצרה או עודכנה במרכז הניהול של Exchange אינה חלה על תיבות דואר או פריטים אינם מועברים לתיבת הדואר של הארכיון או נמחקים.</span><span class="sxs-lookup"><span data-stu-id="215db-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="215db-105">**גורמים בסיסיים:**</span><span class="sxs-lookup"><span data-stu-id="215db-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="215db-106">ייתכן שהסיבה לכך היא **שמסייע התיקיות המנוהלות** לא עיבד את תיבת הדואר של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="215db-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="215db-107">מסייע התיקיות המנוהלות מנסה לעבד כל תיבת דואר בארגון מבוסס הענן שלך פעם בכל שבעה ימים.</span><span class="sxs-lookup"><span data-stu-id="215db-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="215db-108">אם אתה משנה תגית שמירה או מחיל מדיניות שמירה שונה על תיבת דואר, באפשרותך להמתין עד לקבלת סיוע בתיקיה המנוהלת לעיבוד תיבת הדואר, או להפעיל את ה-cmdlet Start-ManagedFolderAssistant כדי להפעיל את מסייע התיקיות המנוהלות כדי לעבד תיבת דואר ספציפית.</span><span class="sxs-lookup"><span data-stu-id="215db-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="215db-109">הפעלת cmdlet זה שימושית לבדיקה או לפתרון בעיות של מדיניות שמירה או הגדרות של תגית שמירה.</span><span class="sxs-lookup"><span data-stu-id="215db-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="215db-110">לקבלת מידע נוסף, בקר [בהפעלת מסייע התיקיות המנוהלות](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="215db-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="215db-111">**הפתרון:** הפעל את הפקודה הבאה כדי להפעיל את מסייע התיקיות המנוהלות עבור תיבת דואר ספציפית:</span><span class="sxs-lookup"><span data-stu-id="215db-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="215db-112">הדבר עשוי להתרחש גם אם **RetentionHold** הפך **לזמין** בתיבת הדואר.</span><span class="sxs-lookup"><span data-stu-id="215db-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="215db-113">אם תיבת הדואר ממוקמת ב-RetentionHold, מדיניות השמירה בתיבת הדואר לא תעובד במהלך זמן זה.</span><span class="sxs-lookup"><span data-stu-id="215db-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="215db-114">לקבלת מידע נוסף על informaton בהגדרה RetentionHold ראה: [החזקת שמירה של תיבת דואר](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="215db-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="215db-115">**פתרון**</span><span class="sxs-lookup"><span data-stu-id="215db-115">**Solution:**</span></span>
    
  - <span data-ttu-id="215db-116">בדוק את מצב ההגדרה RetentionHold בתיבת הדואר הספציפית ב- [קליפת powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="215db-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="215db-117">הפעל את הפקודה הבאה כדי **להפוך את RetentionHold ללא זמין** בתיבת דואר ספציפית:</span><span class="sxs-lookup"><span data-stu-id="215db-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="215db-118">כעת, הפעל מחדש את מסייע התיקיות המנוהלות:</span><span class="sxs-lookup"><span data-stu-id="215db-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="215db-119">**הערה:** אם תיבת דואר קטנה מ-10 MB, מסייע התיקיות המנוהלות לא יעבד באופן אוטומטי את תיבת הדואר.</span><span class="sxs-lookup"><span data-stu-id="215db-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="215db-120">לקבלת מידע נוסף אודות מדיניות שמירה במרכז הניהול של Exchange, ראה:</span><span class="sxs-lookup"><span data-stu-id="215db-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="215db-121">תגי שמירה ומדיניות שמירה</span><span class="sxs-lookup"><span data-stu-id="215db-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="215db-122">החלת מדיניות שמירה על תיבות דואר</span><span class="sxs-lookup"><span data-stu-id="215db-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="215db-123">הוספה או הסרה של תגי שמירה</span><span class="sxs-lookup"><span data-stu-id="215db-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="215db-124">כיצד לזהות את סוג החסימה שתמוקם בתיבת דואר</span><span class="sxs-lookup"><span data-stu-id="215db-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
