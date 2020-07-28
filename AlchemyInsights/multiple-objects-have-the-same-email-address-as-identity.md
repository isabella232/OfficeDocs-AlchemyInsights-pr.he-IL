---
title: לאובייקטים מרובים יש את אותה כתובת דואר אלקטרוני כזהות
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439194"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="def18-102">לאובייקטים מרובים יש את אותה כתובת דואר אלקטרוני כזהות</span><span class="sxs-lookup"><span data-stu-id="def18-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="def18-103">**אובייקטים מרובים**</span><span class="sxs-lookup"><span data-stu-id="def18-103">**Multiple objects**</span></span>

<span data-ttu-id="def18-104">אחת הסיבות השכיחות של שגיאה זו אינה מסוגלת לנתב בקשת Outlook Web Access כראוי בנוכחות אובייקטים מרובים שיש להם אותה כתובת דואר אלקטרוני כזהות.</span><span class="sxs-lookup"><span data-stu-id="def18-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="def18-105">כדי לאתר אובייקטים אלה, הפעל את הפקודות הבאות:</span><span class="sxs-lookup"><span data-stu-id="def18-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="def18-106">· קבל-נמען<email address></span><span class="sxs-lookup"><span data-stu-id="def18-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="def18-107">· קבל-משתמש<email address></span><span class="sxs-lookup"><span data-stu-id="def18-107">· Get-User <email address></span></span>

<span data-ttu-id="def18-108">· משתמש מקבל-משתמש <email address> -סופדלטד</span><span class="sxs-lookup"><span data-stu-id="def18-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="def18-109">· ליצור קשר<email address></span><span class="sxs-lookup"><span data-stu-id="def18-109">· Get-Contact <email address></span></span>

<span data-ttu-id="def18-110">· התיקיה ' קבל-הצבת דואר <email address> '</span><span class="sxs-lookup"><span data-stu-id="def18-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="def18-111">· תיבת דואר שקיבלת-תיבת דואר <email address> -includesoftted</span><span class="sxs-lookup"><span data-stu-id="def18-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="def18-112">· קבל-תיבת דואר <email address> -inactivemailboxonly</span><span class="sxs-lookup"><span data-stu-id="def18-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="def18-113">כדי לפתור את הבעיה, הסר אובייקטים מרובים עם אותה זהות דוא"ל וודא שקיים אובייקט בודד עם זהות הדואר האלקטרוני הספציפית ושסוג הנמען שלו הוא UserMailbox.</span><span class="sxs-lookup"><span data-stu-id="def18-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="def18-114">**אותה כתובת משמשת עבור תיבות דואר של עסקים וצרכנים**</span><span class="sxs-lookup"><span data-stu-id="def18-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="def18-115">סיבה נוספת היא כאשר משתמשים באותה כתובת עבור תיבות דואר של עסקים וצרכנים.</span><span class="sxs-lookup"><span data-stu-id="def18-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="def18-116">במקרה זה, על המשתמש לשנות את כינוי הצרכן העיקרי שלהם עד שבית הקפה תומך בתרחיש זה.</span><span class="sxs-lookup"><span data-stu-id="def18-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="def18-117">זוהי שגיאה קבועה שלא להיעלם ללא התערבות.</span><span class="sxs-lookup"><span data-stu-id="def18-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="def18-118">לפרטים, ראה [שינוי כתובת הדואר האלקטרוני או מספר הטלפון של חשבון Microsoft שברשותך](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="def18-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>