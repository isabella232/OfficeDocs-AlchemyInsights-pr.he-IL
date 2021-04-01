---
title: הגדרת Microsoft Edge כדפדפן ברירת המחדל במכשיר macOS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491554"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="8f043-102">הגדרת Microsoft Edge כדפדפן ברירת המחדל במכשיר macOS</span><span class="sxs-lookup"><span data-stu-id="8f043-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="8f043-103">השתמש באחת משיטות אלה כדי להגדיר את Microsoft Edge כדפדפן ברירת המחדל:</span><span class="sxs-lookup"><span data-stu-id="8f043-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="8f043-104">שיטה 1: הבהב במכשיר עם תמונה של macOS שבו Microsoft Edge כבר הוגדר כדפדפן ברירת המחדל.</span><span class="sxs-lookup"><span data-stu-id="8f043-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="8f043-105">שיטה 2: הגדר את המדיניות DefaultBrowserSettingEnabled כדי לבקש מהמשתמש להגדיר את Microsoft Edge כדפדפן ברירת המחדל.</span><span class="sxs-lookup"><span data-stu-id="8f043-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="8f043-106">אחת מהשיטות מאפשרת למשתמש לשנות את דפדפן ברירת המחדל.</span><span class="sxs-lookup"><span data-stu-id="8f043-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="8f043-107">מסיבה זו, מומלץ לפרוס את המדיניות DefaultBrowserSettingEnabled גם אם השתמשת בשיטה 1.</span><span class="sxs-lookup"><span data-stu-id="8f043-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="8f043-108">אם משתמש משנה את דפדפן ברירת המחדל לאחר פריסת המדיניות, המדיניות מנחה את המשתמש להגדיר את דפדפן ברירת המחדל בחזרה ל- Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="8f043-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
