---
title: הרשאות לוח שנה
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748794"
---
# <a name="calendar-permissions"></a><span data-ttu-id="03e86-102">הרשאות לוח שנה</span><span class="sxs-lookup"><span data-stu-id="03e86-102">Calendar Permissions</span></span>

<span data-ttu-id="03e86-103">משתמשים יכולים לשנות את הרשאות לוח השנה שלהם באמצעות Outlook באינטרנט או לקוחות אחרים, אך כמנהל מערכת, ייתכן שתצטרך גם לחקור אותו.</span><span class="sxs-lookup"><span data-stu-id="03e86-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="03e86-104">באמצעות ה-cmdlet של Exchange PowerShell, תראה את ההרשאה בלוח השנה של המשתמש:</span><span class="sxs-lookup"><span data-stu-id="03e86-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="03e86-105">כדי לראות מידע נוסף, עיין במאמר הבא:</span><span class="sxs-lookup"><span data-stu-id="03e86-105">To see more information see the following:</span></span>

- [<span data-ttu-id="03e86-106">Get-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="03e86-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="03e86-107">Set-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="03e86-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="03e86-108">Add-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="03e86-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="03e86-109">הרשאות לוח שנה משמשות בשיתוף לוחות שנה, כדי לראות מידע נוסף אודות שיתוף לוח שנה של Outlook, עיין במאמרים הבאים:</span><span class="sxs-lookup"><span data-stu-id="03e86-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="03e86-110">שיתוף לוח שנה של Outlook עם אנשים אחרים</span><span class="sxs-lookup"><span data-stu-id="03e86-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="03e86-111">שיתוף לוח השנה שלך ב-Outlook באינטרנט לעסקים</span><span class="sxs-lookup"><span data-stu-id="03e86-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="03e86-112">כדי לפתור בעיות של הרשאת לוח שנה, באפשרותך להשתמש בכלי [מסייע התמיכה והשחזור](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .</span><span class="sxs-lookup"><span data-stu-id="03e86-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>