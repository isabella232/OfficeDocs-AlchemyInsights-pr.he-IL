---
title: 0x8004de40 בעת הפעלת OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813653"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="2f66d-102">0x8004de40 בעת הפעלת OneDrive</span><span class="sxs-lookup"><span data-stu-id="2f66d-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="2f66d-103">אם אתה מקבל הודעת **0x8004de40 בעת** כניסה ל- OneDrive, אתחל מחדש את המחשב בזמן שאתה מחובר לתחום שלך בעבודה או בבית הספר.</span><span class="sxs-lookup"><span data-stu-id="2f66d-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="2f66d-104">אם אתה מקבל שגיאה זו לאחר אתחול מחדש, נסה זאת בזמן שאתה מחובר לתחום שלך בעבודה או בבית הספר:</span><span class="sxs-lookup"><span data-stu-id="2f66d-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="2f66d-105">לחץ על התחל והקלד **cmd** **או שורת פקודה**  בתיבת החיפוש, לחץ באמצעות לחצן העכבר הימני על אפליקציית שורת הפקודה ובחר  **הפעל כמנהל מערכת**.</span><span class="sxs-lookup"><span data-stu-id="2f66d-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="2f66d-106">אם תתבקש לספק סיסמת מנהל מערכת או אישור, הקלד את הסיסמה או לחץ על **אפשר**.</span><span class="sxs-lookup"><span data-stu-id="2f66d-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="2f66d-107">בחלון שורת הפקודה, הקלד **dsregcmd /leave**  ולהמתין להשלמת הפקודה.</span><span class="sxs-lookup"><span data-stu-id="2f66d-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="2f66d-108">לאחר מכן **הקלד dsregcmd /join** ולהמתין להשלמת הפקודה.</span><span class="sxs-lookup"><span data-stu-id="2f66d-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="2f66d-109">אתחל מחדש את המחשב.</span><span class="sxs-lookup"><span data-stu-id="2f66d-109">Reboot your computer.</span></span>
