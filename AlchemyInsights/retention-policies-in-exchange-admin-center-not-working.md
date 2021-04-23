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
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952229"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="f175f-102">מדיניות שמירה במרכז הניהול של Exchange</span><span class="sxs-lookup"><span data-stu-id="f175f-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="f175f-103">אם ברצונך שנריץ בדיקות אוטומטיות עבור ההגדרות שהוזכרו להלן, בחר את לחצן הקודם <- בחלק העליון של דף זה ולאחר מכן הזן את כתובת הדואר האלקטרוני של המשתמש שיש לו בעיות במדיניות שמירה.</span><span class="sxs-lookup"><span data-stu-id="f175f-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="f175f-104">אם אתה נתקל בבעיות במדיניות שמירה במרכז הניהול של Exchange שלא חלות על תיבות דואר או על פריטים שלא עוברים לתיבת הדואר של הארכיון, בדוק את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="f175f-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="f175f-105">**סיבות בסיס:**</span><span class="sxs-lookup"><span data-stu-id="f175f-105">**Root Causes:**</span></span>

- <span data-ttu-id="f175f-106">**מסייע התיקיות** המנוהלים לא עיבד את תיבת הדואר של המשתמש.</span><span class="sxs-lookup"><span data-stu-id="f175f-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="f175f-107">מסייע התיקיות המנוהלים מנסה לעבד כל תיבת דואר בארגון המבוסס על ענן צמתים פעם בשבעה ימים.</span><span class="sxs-lookup"><span data-stu-id="f175f-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="f175f-108">**הפתרון:** הפעל את מסייע התיקיות המנוהלים.</span><span class="sxs-lookup"><span data-stu-id="f175f-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="f175f-109">**RetentionHold** הופעל **בתיבת** הדואר.</span><span class="sxs-lookup"><span data-stu-id="f175f-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="f175f-110">אם תיבת הדואר ממוקמת ב- RetentionHold, מדיניות השמירה בתיבת הדואר לא תעובד במהלך זמן זה.</span><span class="sxs-lookup"><span data-stu-id="f175f-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="f175f-111">**הפתרון:** בדוק את המצב של הגדרת החזקת שמירה ועדכן אותו כצורך.</span><span class="sxs-lookup"><span data-stu-id="f175f-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="f175f-112">לקבלת פרטים, ראה [החזקת שמירת תיבת דואר](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="f175f-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="f175f-113">**הערה:** אם תיבת דואר קטנה מ- 10 MB, מסייע התיקיות המנוהלים לא יעבד באופן אוטומטי את תיבת הדואר.</span><span class="sxs-lookup"><span data-stu-id="f175f-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="f175f-114">לקבלת מידע נוסף על מדיניות שמירה במרכז הניהול של Exchange, ראה:</span><span class="sxs-lookup"><span data-stu-id="f175f-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="f175f-115">תגיות שמירה ומדיניות שמירה</span><span class="sxs-lookup"><span data-stu-id="f175f-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="f175f-116">[החלת מדיניות שמירה על תיבות דואר או](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) [הוספה או הסרה של תגיות שמירה](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="f175f-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="f175f-117">כיצד לזהות את סוג הה להחזיק בתיבת דואר</span><span class="sxs-lookup"><span data-stu-id="f175f-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
