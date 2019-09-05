---
title: אין אפשרות למחוק פריטים ב-SharePoint או OneDrive
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3cc168846999c6880b95edfaedb2df8cf6e843a6
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36748558"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="ba030-102">אין אפשרות למחוק פריטים</span><span class="sxs-lookup"><span data-stu-id="ba030-102">Unable to delete items</span></span>

<span data-ttu-id="ba030-103">האם יש בעיות במחיקת פריטי SharePoint?</span><span class="sxs-lookup"><span data-stu-id="ba030-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="ba030-104">ודא תמיד שיש לך את [ההרשאות המתאימות](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) למחיקת הפריט או [שמנהל אוסף אתרים](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) ינסה להסיר את הפריט.</span><span class="sxs-lookup"><span data-stu-id="ba030-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="ba030-105">ודא שלא קיימת הגדרת [מדיניות שמירה](https://docs.microsoft.com/office365/securitycompliance/retention-policies) בפריט.</span><span class="sxs-lookup"><span data-stu-id="ba030-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="ba030-106">ודא שהפריט לא [הוצא](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) למשתמש אחר.</span><span class="sxs-lookup"><span data-stu-id="ba030-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="ba030-107">לבסוף, מנהלי מערכת יכולים להשתמש [בתבניות ובשיטות](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) עבודה של SharePoint (PnP) המכילים ספריה של פקודות PowerShell המאפשרות לך לבצע פעולות ניהול מורכבות כגון כפיית מחיקת פריטים עקשנים.</span><span class="sxs-lookup"><span data-stu-id="ba030-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="ba030-108">הסר קובץ PNP</span><span class="sxs-lookup"><span data-stu-id="ba030-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="ba030-109">הסר תיקיית PNP</span><span class="sxs-lookup"><span data-stu-id="ba030-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="ba030-110">הסר פריט רשימת PNP</span><span class="sxs-lookup"><span data-stu-id="ba030-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="ba030-111">הסר רשימת PNP</span><span class="sxs-lookup"><span data-stu-id="ba030-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="ba030-112">הסר שדה PNP (עמודה)</span><span class="sxs-lookup"><span data-stu-id="ba030-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)