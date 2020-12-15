---
title: הסרת גירסאות קודמות של MSI של Office
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003886"
- "6940"
ms.openlocfilehash: 26ab610cb204149536bd23c830a1b8558892a7c0
ms.sourcegitcommit: c033720921cb9a06b9560eedef4f1935e69a846b
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/15/2020
ms.locfileid: "49680687"
---
# <a name="remove-prior-msi-versions-of-office"></a><span data-ttu-id="3e38e-102">הסרת גירסאות קודמות של MSI של Office</span><span class="sxs-lookup"><span data-stu-id="3e38e-102">Remove prior MSI versions of Office</span></span>

<span data-ttu-id="3e38e-103">אני ממליץ על הסרת גירסאות קודמות של Windows Installer (MSI) של Office לפני התקנת Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="3e38e-103">I recommend removing prior Windows Installer (MSI) versions of Office before installing Office 365 ProPlus.</span></span> <span data-ttu-id="3e38e-104">כך ניתן לעשות זאת:</span><span class="sxs-lookup"><span data-stu-id="3e38e-104">Here's how to do this:</span></span>

1. <span data-ttu-id="3e38e-105">אם השתמשת ב-MSI כדי להתקין את Office, באפשרותך להשתמש בכלי הפריסה של Office (ODT) כדי להסיר את התקנת Office.</span><span class="sxs-lookup"><span data-stu-id="3e38e-105">If you used MSI to install Office, you can use the Office Deployment Tool (ODT) to uninstall Office.</span></span> <span data-ttu-id="3e38e-106">באפשרותך להשתמש ברכיב RemoveMSI בקובץ **הconfiguration.xml** שלך.</span><span class="sxs-lookup"><span data-stu-id="3e38e-106">You can use the RemoveMSI element in your **configuration.xml** file.</span></span>
1. <span data-ttu-id="3e38e-107">בצע את ההוראות במאמר זה: [מרכז התאימות & אבטחה של Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="3e38e-107">Follow the instruction in this article: [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span></span>