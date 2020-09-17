---
title: העברת הודעות דואר אלקטרוני לתיבת הדואר של הארכיון
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799781"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="580fb-102">העברת דואר אלקטרוני לתיבת הדואר של הארכיון</span><span class="sxs-lookup"><span data-stu-id="580fb-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="580fb-103">אם ברצונך לבצע בדיקות אוטומטיות עבור ההגדרות המוזכרות להלן, בחר את לחצן ' הקודם ' < '-בחלק העליון של דף זה ולאחר מכן הזן את כתובת הדואר האלקטרוני של המשתמש שנתקל בבעיות בהעברת דואר אלקטרוני לתיבת הדואר של הארכיון.</span><span class="sxs-lookup"><span data-stu-id="580fb-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="580fb-104">ודא **שתיבת דואר של ארכיון** הופעלה.</span><span class="sxs-lookup"><span data-stu-id="580fb-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="580fb-105">אם לא, השתמש בשלבים המפורטים [במאמר זה](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) כדי להפוך את תיבת הדואר של הארכיון לזמינה.</span><span class="sxs-lookup"><span data-stu-id="580fb-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="580fb-106">כדי לאחסן בארכיון הודעות באופן אוטומטי בתיבת הדואר של הארכיון, יש להגדיר תגית שמירה עם הפעולה ' **העבר לארכיון** ' כדי **להחיל אותה באופן אוטומטי על התגית תיבת דואר מלאה (ברירת מחדל)**.</span><span class="sxs-lookup"><span data-stu-id="580fb-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="580fb-107">השתמש בשלבים הבאים כדי ליצור את התגית: [תג ברירת המחדל של הארכיון](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="580fb-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="580fb-108">לאחר מכן, הוסף את תג **הארכיון** למדיניות השמירה.</span><span class="sxs-lookup"><span data-stu-id="580fb-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="580fb-109">במרכז הניהול של Exchange, בחר **מדיניות שמירה** > הוסף את **התגית ' העבר לארכיון** ' למדיניות > **Save**.</span><span class="sxs-lookup"><span data-stu-id="580fb-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="580fb-110">כעת [הקצה את מדיניות השמירה](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) לתיבת הדואר של המשתמש הספציפי.</span><span class="sxs-lookup"><span data-stu-id="580fb-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="580fb-111">מדיניות זו תחול על תיבת הדואר **הראשית** והן עבור תיבת הדואר של **הארכיון** .</span><span class="sxs-lookup"><span data-stu-id="580fb-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="580fb-112">ייתכן שיהיה צורך לאלץ את מסייע התיקיות המנוהלות (מנהל המשרד) לפעול ולהחיל את ההגדרות החדשות על תיבת הדואר של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="580fb-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="580fb-113">הפעל את הפקודה הבאה כאשר אתה [מחובר ל-קליפת PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) כדי להפעיל את מסייע התיקיות המנוהלות עבור תיבת דואר ספציפית:</span><span class="sxs-lookup"><span data-stu-id="580fb-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="580fb-114">Start-ManagedFolderAssistant-זהות <name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="580fb-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="580fb-115">לקבלת מידע נוסף אודות הגדרת מדיניות ארכיון, ראה [הגדרת מדיניות ארכיון ומחיקה עבור תיבות דואר](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="580fb-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  