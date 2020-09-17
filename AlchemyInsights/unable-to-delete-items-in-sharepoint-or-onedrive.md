---
title: אין אפשרות למחוק פריטים ב-SharePoint או ב-OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: fd12115214cc28b822cf7fa57fe9b86f76f7beb1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806112"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="ff1ce-102">לא ניתן למחוק פריטים</span><span class="sxs-lookup"><span data-stu-id="ff1ce-102">Unable to delete items</span></span>

<span data-ttu-id="ff1ce-103">מדיניות שמירה יכולה לגרום לכך, עליך להפוך ללא זמין או לא לכלול החזקה שגורמת לבעיה זו.</span><span class="sxs-lookup"><span data-stu-id="ff1ce-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="ff1ce-104">לאחר הסרת מדיניות שמירה או חסימה, ייתכן שיחלפו עד 24 שעות כדי שהשינוי ייכנס לתוקף.</span><span class="sxs-lookup"><span data-stu-id="ff1ce-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="ff1ce-105">ודא שאין הגדרת [מדיניות שמירה](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) על הפריט.</span><span class="sxs-lookup"><span data-stu-id="ff1ce-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="ff1ce-106">ייתכן שהאתר חרג ממגבלת האחסון, הגדל את [מיכסת האתר](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) ומחק את הפריט.</span><span class="sxs-lookup"><span data-stu-id="ff1ce-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="ff1ce-107">ודא שהפריט לא [הוצא](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) למשתמש אחר.</span><span class="sxs-lookup"><span data-stu-id="ff1ce-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="ff1ce-108">בסופו של דבר, מנהלי מערכת יכולים להשתמש [בתבניות ובתרגולים של SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) אשר מכילים ספריה של פקודות PowerShell המאפשרות לך לבצע פעולות ניהול מורכבות כגון כפה על מחיקת פריטים עקשניים.</span><span class="sxs-lookup"><span data-stu-id="ff1ce-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="ff1ce-109">הסרת קובץ PNP</span><span class="sxs-lookup"><span data-stu-id="ff1ce-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="ff1ce-110">הסרת תיקיית PNP</span><span class="sxs-lookup"><span data-stu-id="ff1ce-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="ff1ce-111">הסרת פריט רשימה של PNP</span><span class="sxs-lookup"><span data-stu-id="ff1ce-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="ff1ce-112">הסרת רשימת PNP</span><span class="sxs-lookup"><span data-stu-id="ff1ce-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="ff1ce-113">הסרת שדה PNP (עמודה)</span><span class="sxs-lookup"><span data-stu-id="ff1ce-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)