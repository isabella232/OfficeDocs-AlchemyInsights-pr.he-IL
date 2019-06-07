---
title: העברת הודעות דואר אלקטרוני בתיבת הדואר של ארכיון
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: fb5745b60d42e1f7d7bb9b7a336a51b62c2ff92a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762366"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="6fd4a-102">העבר דואר אלקטרוני בתיבת הדואר של ארכיון</span><span class="sxs-lookup"><span data-stu-id="6fd4a-102">Move email to the archive mailbox</span></span>
 
1. <span data-ttu-id="6fd4a-103">ודא כי **לאחסן בארכיון דואר** הפכה לזמינה.</span><span class="sxs-lookup"><span data-stu-id="6fd4a-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="6fd4a-104">אם לא, בצע את הפעולות במאמר [זה](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) כדי להפעיל את תיבת הדואר של ארכיון.</span><span class="sxs-lookup"><span data-stu-id="6fd4a-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="6fd4a-105">כדי לאחסן בארכיון הודעות באופן אוטומטי תיבת הדואר של ארכיון, יש להגדיר תג שמירה עם פעולת **העבר לאחסן בארכיון** כדי **להחיל באופן אוטומטי על תג תיבת הדואר כולה (ברירת המחדל)**.</span><span class="sxs-lookup"><span data-stu-id="6fd4a-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="6fd4a-106">השתמש בשלבים כאן כדי ליצור את התג: [תג ברירת מחדל של ארכיון](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span><span class="sxs-lookup"><span data-stu-id="6fd4a-106">Use the steps here to create the tag: [Archive Default tag](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span></span>
    
3. <span data-ttu-id="6fd4a-107">לאחר מכן, הוסף את תג **ארכיון** למדיניות השמירה שלך.</span><span class="sxs-lookup"><span data-stu-id="6fd4a-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="6fd4a-108">במרכז הניהול של Exchange, בחר **מדיניות שמירה** > להוסיף **לקליפ תג ארכיון** > מדיניות **שמירה**.</span><span class="sxs-lookup"><span data-stu-id="6fd4a-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span> 
    
4. <span data-ttu-id="6fd4a-109">כעת [להקצות מדיניות השמירה](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) תיבת דואר של משתמש מסוים.</span><span class="sxs-lookup"><span data-stu-id="6fd4a-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="6fd4a-110">באותה המדיניות יוחלו על **ראשי** וגם את תיבת הדואר של **ארכיון** .</span><span class="sxs-lookup"><span data-stu-id="6fd4a-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="6fd4a-111">ייתכן שיהיה עליך לכפות את מנוהל תיקיה המסייע (MFA) כדי להפעיל, להחיל את ההגדרות החדשות לתיבת הדואר של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="6fd4a-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="6fd4a-112">הפעל את הפקודה הבאה בעת [מחובר EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) כדי להפעיל את ניהול מסייע התיקיות עבור תיבת דואר מסוימת:</span><span class="sxs-lookup"><span data-stu-id="6fd4a-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="6fd4a-113">לקבלת מידע נוסף אודות הגדרת מדיניות אחסון בארכיון, ראה [הגדרת מדיניות ארכיון ומחיקה של תיבות דואר](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="6fd4a-113">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

