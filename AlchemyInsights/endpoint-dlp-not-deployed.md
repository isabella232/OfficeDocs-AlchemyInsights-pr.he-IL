---
title: DLP של נקודת קצה לא נפרס במכשיר של המשתמש
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731585"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a><span data-ttu-id="3794f-102">DLP של נקודת קצה לא נפרס במכשיר של המשתמש</span><span class="sxs-lookup"><span data-stu-id="3794f-102">Endpoint DLP not deployed to user's device</span></span>

<span data-ttu-id="3794f-103">אם ההגדרה מניעת אובדן נתונים של נקודת קצה (DLP) לא חלה על מכשיר של משתמש, אשר שאתה מביע את הדרישות הבאות:</span><span class="sxs-lookup"><span data-stu-id="3794f-103">If the Endpoint data loss prevention (DLP) setting has not applied to a user's device, confirm you meet these requirements:</span></span>

- <span data-ttu-id="3794f-104">Windows 10 x64 גירסת Build מס' 1809 ואילך מותקנת במכשיר.</span><span class="sxs-lookup"><span data-stu-id="3794f-104">Windows 10 x64 build 1809 or later is installed on the device.</span></span>
- <span data-ttu-id="3794f-105">לקוח נגד תוכנות זדוניות גירסה 4.18.2009.7 ואילך מותקן.</span><span class="sxs-lookup"><span data-stu-id="3794f-105">Anti-malware client version 4.18.2009.7 or later is installed.</span></span>
- <span data-ttu-id="3794f-106">המכשיר הוא **אחד** מאלה:</span><span class="sxs-lookup"><span data-stu-id="3794f-106">The device is **one** of these:</span></span>
    
    - <span data-ttu-id="3794f-107">Azure Active Directory (Azure AD) מצורף</span><span class="sxs-lookup"><span data-stu-id="3794f-107">Azure Active Directory (Azure AD) joined</span></span>
    - <span data-ttu-id="3794f-108">Azure AD היברידי מצורף</span><span class="sxs-lookup"><span data-stu-id="3794f-108">Hybrid Azure AD joined</span></span>
    - <span data-ttu-id="3794f-109">AAD רשום</span><span class="sxs-lookup"><span data-stu-id="3794f-109">AAD registered</span></span>

- <span data-ttu-id="3794f-110">כדי לאכוף פעולות מדיניות, ודא שדפדפן Microsoft Chromium Edge מותקן במכשיר נקודת הקצה.</span><span class="sxs-lookup"><span data-stu-id="3794f-110">To enforce policy actions, make sure Microsoft Chromium Edge browser is installed on the endpoint device.</span></span>

<span data-ttu-id="3794f-111">לקבלת דרישות נוספות לפריסת DLP של נקודת קצה, ראה [תחילת העבודה עם מניעת אובדן נתונים של נקודת קצה](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span><span class="sxs-lookup"><span data-stu-id="3794f-111">For additional requirements for deploying Endpoint DLP, see [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span></span>