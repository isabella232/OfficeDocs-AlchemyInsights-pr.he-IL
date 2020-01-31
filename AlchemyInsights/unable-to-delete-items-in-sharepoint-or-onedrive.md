---
title: אין אפשרות למחוק פריטים ב-SharePoint או OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571258"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="96b0f-102">אין אפשרות למחוק פריטים</span><span class="sxs-lookup"><span data-stu-id="96b0f-102">Unable to delete items</span></span>

<span data-ttu-id="96b0f-103">מדיניות שמירה עלולה לגרום לכך, עליך לבטל או להוציא החזקה בהתאמה שגורמת לבעיה זו.</span><span class="sxs-lookup"><span data-stu-id="96b0f-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="96b0f-104">לאחר הסרת מדיניות שמירה או החזקה, ייתכן שהשינוי ישפיע עד 24 שעות.</span><span class="sxs-lookup"><span data-stu-id="96b0f-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="96b0f-105">ודא שלא קיימת הגדרת [מדיניות שמירה](https://docs.microsoft.com/office365/securitycompliance/retention-policies) בפריט.</span><span class="sxs-lookup"><span data-stu-id="96b0f-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="96b0f-106">ייתכן שהאתר חרג ממגבלת האחסון, הגדל את [מיכסת האתר](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) ומחק את הפריט.</span><span class="sxs-lookup"><span data-stu-id="96b0f-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="96b0f-107">ודא שהפריט לא [הוצא](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) למשתמש אחר.</span><span class="sxs-lookup"><span data-stu-id="96b0f-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="96b0f-108">לבסוף, מנהלי מערכת יכולים להשתמש [בתבניות ובשיטות](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) עבודה של SharePoint (PnP) המכילים ספריה של פקודות PowerShell המאפשרות לך לבצע פעולות ניהול מורכבות כגון כפיית מחיקת פריטים עקשנים.</span><span class="sxs-lookup"><span data-stu-id="96b0f-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="96b0f-109">הסר קובץ PNP</span><span class="sxs-lookup"><span data-stu-id="96b0f-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="96b0f-110">הסר תיקיית PNP</span><span class="sxs-lookup"><span data-stu-id="96b0f-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="96b0f-111">הסר פריט רשימת PNP</span><span class="sxs-lookup"><span data-stu-id="96b0f-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="96b0f-112">הסר רשימת PNP</span><span class="sxs-lookup"><span data-stu-id="96b0f-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="96b0f-113">הסר שדה PNP (עמודה)</span><span class="sxs-lookup"><span data-stu-id="96b0f-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)