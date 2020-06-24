---
title: הרשאות לוח שנה
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862094"
---
# <a name="calendar-permissions"></a><span data-ttu-id="b1769-102">הרשאות לוח שנה</span><span class="sxs-lookup"><span data-stu-id="b1769-102">Calendar Permissions</span></span>

<span data-ttu-id="b1769-103">משתמשים יכולים לשנות את הרשאות לוח השנה שלהם עם Outlook באינטרנט או לקוחות אחרים, אך כמנהל ייתכן שיהיה עליך לחקור גם כן.</span><span class="sxs-lookup"><span data-stu-id="b1769-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="b1769-104">ב-cmdlet של Exchange PowerShell יציג את ההרשאה בלוח השנה של המשתמש:</span><span class="sxs-lookup"><span data-stu-id="b1769-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="b1769-105">כדי לראות מידע נוסף, עיין בפרטים הבאים:</span><span class="sxs-lookup"><span data-stu-id="b1769-105">To see more information see the following:</span></span>

- [<span data-ttu-id="b1769-106">הרשאת קבלת-Mailboxbox</span><span class="sxs-lookup"><span data-stu-id="b1769-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="b1769-107">הרשאת הגדרת דואר אלקטרוני</span><span class="sxs-lookup"><span data-stu-id="b1769-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="b1769-108">הרשאת הוספת בתיבת דואר</span><span class="sxs-lookup"><span data-stu-id="b1769-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="b1769-109">הרשאות לוח שנה משמשות בשיתוף לוחות שנה, כדי לראות מידע נוסף אודות שיתוף לוח שנה של Outlook, עיין במאמרים אלה:</span><span class="sxs-lookup"><span data-stu-id="b1769-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="b1769-110">שיתוף לוח שנה של Outlook עם אנשים אחרים</span><span class="sxs-lookup"><span data-stu-id="b1769-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="b1769-111">שיתוף לוח השנה שלך ב-Outlook באינטרנט עבור עסקים</span><span class="sxs-lookup"><span data-stu-id="b1769-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="b1769-112">כדי לפתור בעיות בהרשאת לוח שנה, באפשרותך להשתמש בכלי [מסייע התמיכה והשחזור](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .</span><span class="sxs-lookup"><span data-stu-id="b1769-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>