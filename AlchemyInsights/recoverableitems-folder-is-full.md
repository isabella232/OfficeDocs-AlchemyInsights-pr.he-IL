---
title: 1336 התיקיה ' פריטים להתאוששות ' מלאה
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720253"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="1f7ae-102">התיקיה ' פריטים הניתנים לשחזור ' מלאה</span><span class="sxs-lookup"><span data-stu-id="1f7ae-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="1f7ae-103">עבור תיבות דואר של Exchange Online, מגבלת האחסון המהווה ברירת מחדל עבור התיקיה ' פריטים הניתנים לשחזור ' היא 30 GB.</span><span class="sxs-lookup"><span data-stu-id="1f7ae-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="1f7ae-104">מגבלת האחסון עבור התיקיה ' פריטים הניתנים לשחזור ' מוגברת באופן אוטומטי ל-100 GB אם תיבת הדואר ממוקמת בחסימה משפטית, החזקת eDiscovery, או מוקצית למדיניות שמירה.</span><span class="sxs-lookup"><span data-stu-id="1f7ae-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="1f7ae-105">כאשר התיקיה ' פריטים הניתנים לשחזור ' מגיעה למגבלת האחסון, פונקציונליות תיבת הדואר מושפעת מהדרכים הבאות:</span><span class="sxs-lookup"><span data-stu-id="1f7ae-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="1f7ae-106">למשתמש אין אפשרות למחוק פריטים מתיבת הדואר.</span><span class="sxs-lookup"><span data-stu-id="1f7ae-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="1f7ae-107">למסייע התיקיות המנוהלות אין אפשרות למחוק פריטים לפי תגית שמירה או הגדרות של תיקיות מנוהלות.</span><span class="sxs-lookup"><span data-stu-id="1f7ae-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="1f7ae-108">עבור תיבות דואר שבהן שחזור פריט יחיד מאופשר או ממוקמות בהמתנה, תהליך ההגנה על עמוד ההעתקה מפני כתיבה אינו יכול לשמור על גירסאות של פריטים שנערכו על-ידי המשתמש.</span><span class="sxs-lookup"><span data-stu-id="1f7ae-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="1f7ae-109">עבור תיבות דואר שבהן מופעל רישום ביקורת של תיבת דואר, לא ניתן לשמור ערכי יומן רישום של ביקורת דואר בתיקיית המשנה ' ביקורת ' בתיקיה ' פריטים הניתנים לשחזור '.</span><span class="sxs-lookup"><span data-stu-id="1f7ae-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="1f7ae-110">עבור תיבות דואר שאינן נמצאות בהמתנה, מנהלים `Search-Mailbox -SearchDumpsterOnly -DeleteContent` יכולים להשתמש בפקודה Exchange Online PowerShell כדי למחוק פריטים בתיקיה פריטים הניתנים לשחזור.</span><span class="sxs-lookup"><span data-stu-id="1f7ae-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="1f7ae-111">כדי לקבל מידע נוסף עיין בנושאים הבאים:</span><span class="sxs-lookup"><span data-stu-id="1f7ae-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="1f7ae-112">חיפוש ומחיקה של הודעות</span><span class="sxs-lookup"><span data-stu-id="1f7ae-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="1f7ae-113">חיפוש-תיבת דואר</span><span class="sxs-lookup"><span data-stu-id="1f7ae-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="1f7ae-114">עבור תיבות דואר הנמצאות בהמתנה, למנהלים יש להסיר את החסימה לפני שהם יכולים למחוק פריטים מהתיקיה ' פריטים הניתנים לשחזור '.</span><span class="sxs-lookup"><span data-stu-id="1f7ae-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="1f7ae-115">לקבלת מידע נוסף, ראה [מחיקת פריטים בתיקיה ' פריטים הניתנים לשחזור ' של תיבות דואר המבוססות על ענן צמתים בהמתנה](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="1f7ae-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="1f7ae-116">כדי לסייע במניעת הגדלת התיקיה ' פריטים הניתנים לשחזור ', מנהלים יכולים להגדיל את מגבלת האחסון של התיקיה ' פריטים הניתנים לשחזור ' עבור תיבות דואר בהמתנה ולהגדיר מדיניות שמירה של תיבת דואר המעביר פריטים מהתיקיה ' פריטים הניתנים לשחזור ' לתיבת הדואר של המשתמש בארכיון.</span><span class="sxs-lookup"><span data-stu-id="1f7ae-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="1f7ae-117">ראה [הגדלת המיכסה של ' פריטים הניתנים לשחזור ' עבור תיבות דואר בהמתנה](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="1f7ae-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
