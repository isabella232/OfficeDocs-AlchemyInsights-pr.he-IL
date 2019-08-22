---
title: התיקיה RecoverableItems 1336 הוא מלא
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 8a5859ba29d847606e8b44d169c3cd6a26364744
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36509739"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="2d1b0-102">התיקיה פריטים ניתנים לשחזור הוא מלא</span><span class="sxs-lookup"><span data-stu-id="2d1b0-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="2d1b0-103">עבור תיבות דואר Exchange Online ב- Office 365, מגבלת האחסון המוגדר כברירת מחדל עבור התיקיה פריטים ניתנים לשחזור הוא 30 ג'יגה-בתים.</span><span class="sxs-lookup"><span data-stu-id="2d1b0-103">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="2d1b0-104">מגבלת האחסון עבור התיקיה פריטים ניתנים לשחזור באופן אוטומטי יגדל עד 100 ג'יגה-בתים אם תיבת הדואר ממוקם על החזק תביעה משפטית, גילוי אלקטרוני בהמתנה, או מוקצה למדיניות השמירה של Office 365.</span><span class="sxs-lookup"><span data-stu-id="2d1b0-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>

<span data-ttu-id="2d1b0-105">כאשר התיקיה פריטים ניתנים לשחזור הגיע למגבלת האחסון, פונקציונליות תיבת הדואר מושפע בדרכים הבאות:</span><span class="sxs-lookup"><span data-stu-id="2d1b0-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="2d1b0-106">למשתמש אין אפשרות למחוק פריטים מתיבת הדואר.</span><span class="sxs-lookup"><span data-stu-id="2d1b0-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="2d1b0-107">מנוהל מסייע התיקיות אין אפשרות למחוק פריטים לפי תגית שמירה או הגדרות תיקיות מנוהלות.</span><span class="sxs-lookup"><span data-stu-id="2d1b0-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="2d1b0-108">עבור תיבות דואר זמין שחזור פריט יחיד או ממוקמים בהמתנה, תהליך הגנת עמוד עותק בעת כתיבה לא ניתן לשמור על גירסאות של פריטים שנערכו על-ידי המשתמש.</span><span class="sxs-lookup"><span data-stu-id="2d1b0-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="2d1b0-109">עבור תיבות דואר שיש להם תיבת דואר ביקורת הרישום זמין, ניתן לשמור ללא ערכי יומן ביקורת של תיבת דואר בתיקיית המשנה ביקורות בתיקיה פריטים ניתנים לשחזור.</span><span class="sxs-lookup"><span data-stu-id="2d1b0-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="2d1b0-110">עבור תיבות דואר שאינן בהמתנה, מנהלים יכולים להשתמש `Search-Mailbox -SearchDumpsterOnly -DeleteContent` הפקודה ב- Exchange Online PowerShell למחיקת פריטים בתיקיה פריטים ניתנים לשחזור.</span><span class="sxs-lookup"><span data-stu-id="2d1b0-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="2d1b0-111">כדי לקבל מידע נוסף עיין בנושאים הבאים:</span><span class="sxs-lookup"><span data-stu-id="2d1b0-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="2d1b0-112">חיפוש ומחיקה של הודעות</span><span class="sxs-lookup"><span data-stu-id="2d1b0-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="2d1b0-113">חיפוש-תיבת דואר</span><span class="sxs-lookup"><span data-stu-id="2d1b0-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="2d1b0-114">עבור תיבות דואר הנמצאות בהמתנה, המנהלים צריך להסיר את החסימה לפני שהם יכולים פריטים שנמחקו מהתיקיה פריטים ניתנים לשחזור.</span><span class="sxs-lookup"><span data-stu-id="2d1b0-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="2d1b0-115">לקבלת מידע נוסף, ראה [מחיקת פריטים בפריטים ניתן לשחזר תיקיה של תיבות דואר מבוססות ענן על החזק](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="2d1b0-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="2d1b0-116">כדי לסייע למנוע את התיקיה פריטים ניתנים לשחזור והופך מלאה, מנהלים באפשרותך להגדיל את המגבלה אחסון של פריטים ניתנים לשחזור תיקיה עבור תיבות דואר על החזק ולהגדיר את מדיניות השמירה תיבת הדואר המעביר פריטים מהתיקיה פריטים ניתנים לשחזור לארכיון של המשתמש תיבת הדואר.</span><span class="sxs-lookup"><span data-stu-id="2d1b0-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="2d1b0-117">ראה [להגדיל פריטים ניתנים לשחזור החזק מיכסה עבור תיבות דואר ב-](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="2d1b0-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
