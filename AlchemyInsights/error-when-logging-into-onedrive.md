---
title: שגיאת 0x8004de40 בעת הפעלת OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823049"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="d32a7-102">שגיאת 0x8004de40 בעת הפעלת OneDrive</span><span class="sxs-lookup"><span data-stu-id="d32a7-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="d32a7-103">אם אתה מקבל הודעת שגיאה **0x8004de40** בעת כניסה ל-OneDrive, אתחל מחדש את המחשב בזמן שאתה מחובר לתחום בעבודה או בבית הספר.</span><span class="sxs-lookup"><span data-stu-id="d32a7-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="d32a7-104">אם אתה מקבל שגיאה זו לאחר אתחול מחדש, נסה זאת בזמן שאתה מחובר לתחום בעבודה או בבית הספר:</span><span class="sxs-lookup"><span data-stu-id="d32a7-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="d32a7-105">לחץ על התחל והקלד **cmd** או **שורת פקודה**  בתיבת החיפוש, לחץ באמצעות לחצן העכבר הימני על יישום שורת הפקודה ובחר  **הפעל כמנהל** .</span><span class="sxs-lookup"><span data-stu-id="d32a7-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="d32a7-106">אם אתה מתבקש להזין סיסמת מנהל מערכת או אישור, הקלד את הסיסמה או לחץ על **אפשר** .</span><span class="sxs-lookup"><span data-stu-id="d32a7-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="d32a7-107">בחלון שורת הפקודה, הקלד **dsregcmd/leave**  והמתן להשלמת הפקודה.</span><span class="sxs-lookup"><span data-stu-id="d32a7-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="d32a7-108">לאחר מכן הקלד **dsregcmd/join** והמתן להשלמת הפקודה.</span><span class="sxs-lookup"><span data-stu-id="d32a7-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="d32a7-109">הפעל מחדש את המחשב.</span><span class="sxs-lookup"><span data-stu-id="d32a7-109">Reboot your computer.</span></span>
