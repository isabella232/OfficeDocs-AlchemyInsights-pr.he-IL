---
title: שנה את Microsoft Edge באמצעות משתני מדריך הנתונים במקום נתיבים של קשיח
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 5c40aa1d7f61fbd2842839a5839899af8ab439f2
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677991"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a><span data-ttu-id="99766-102">שנה את Microsoft Edge באמצעות משתני מדריך הנתונים במקום נתיבים של קשיח</span><span class="sxs-lookup"><span data-stu-id="99766-102">Modify Microsoft Edge by using data directory variables rather than hardcoded paths</span></span>

<span data-ttu-id="99766-103">לדוגמה, ב-Windows, כדי לאחסן את נתוני הפרופיל תחת נתוני היישום המקומי של המשתמש, במקום במיקום ברירת המחדל, הגדר את מדיניות **UserDataDir** ל- **$ {local_app_data} \Edge\Profile**.</span><span class="sxs-lookup"><span data-stu-id="99766-103">For example, on Windows, to store the profile data under a user's local application data rather than in the default location, set the **UserDataDir** policy to **${local_app_data}\Edge\Profile**.</span></span> 

<span data-ttu-id="99766-104">לקבלת מידע נוסף, ראה [יצירת משתני מדריך נתונים של משתמשים ב-Microsoft Edge](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).</span><span class="sxs-lookup"><span data-stu-id="99766-104">To learn more, see [Create Microsoft Edge user data directory variables](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).</span></span>