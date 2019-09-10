---
title: העברת הודעות דואר אלקטרוני לתיבת הדואר ' ארכיון '
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822163"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="ffde8-102">העברת דואר אלקטרוני לתיבת הדואר של הארכיון</span><span class="sxs-lookup"><span data-stu-id="ffde8-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="ffde8-103">ודא **שתיבת דואר של ארכיון** הופעלה.</span><span class="sxs-lookup"><span data-stu-id="ffde8-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="ffde8-104">אם לא, השתמש בשלבים [שבמאמר זה](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) כדי להפוך את תיבת הדואר של הארכיון לזמינה.</span><span class="sxs-lookup"><span data-stu-id="ffde8-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="ffde8-105">כדי לאחסן בארכיון הודעות באופן אוטומטי לתיבת הדואר של הארכיון, יש להגדיר תג שמירה עם **העברת לפעולה בארכיון** כך **שיוחל באופן אוטומטי על תג תיבת הדואר המלא (ברירת המחדל)**.</span><span class="sxs-lookup"><span data-stu-id="ffde8-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="ffde8-106">השתמש בשלבים כאן כדי ליצור את התג: [התגית ' ברירת מחדל של ארכיון](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)'.</span><span class="sxs-lookup"><span data-stu-id="ffde8-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="ffde8-107">לאחר מכן, הוסף את תג **הארכיון** למדיניות השמירה.</span><span class="sxs-lookup"><span data-stu-id="ffde8-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="ffde8-108">במרכז הניהול של Exchange, בחר באפשרות **מדיניות שמירה** _ gtie הוסף את **המעבר לתגית ארכיון** למדיניות _ **שמור**.</span><span class="sxs-lookup"><span data-stu-id="ffde8-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="ffde8-109">כעת [הקצה את מדיניות השמירה](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) לתיבת הדואר של המשתמש הספציפי.</span><span class="sxs-lookup"><span data-stu-id="ffde8-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="ffde8-110">אותה מדיניות תוחל הן על תיבת הדואר **הראשית** והן של **הארכיון** .</span><span class="sxs-lookup"><span data-stu-id="ffde8-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="ffde8-111">ייתכן שיהיה צורך לכפות על מסייע התיקיות המנוהלות (משרד המשנה) להפעיל ולהחיל את ההגדרות החדשות על תיבת הדואר של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="ffde8-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="ffde8-112">הפעל את הפקודה הבאה בעת [ההתחברות ל-EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) כדי להפעיל את מסייע התיקיות המנוהלות עבור תיבת דואר ספציפית:</span><span class="sxs-lookup"><span data-stu-id="ffde8-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="ffde8-113">מסייע מניהול התחל-זהות<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="ffde8-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="ffde8-114">לקבלת מידע נוסף אודות הגדרת מדיניות ארכיון, ראה [הגדרת מדיניות ארכיון ומחיקה עבור תיבות דואר](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="ffde8-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  