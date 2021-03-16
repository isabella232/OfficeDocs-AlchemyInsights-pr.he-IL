---
title: הסרת שירות הרקע עבור Microsoft Search ב-Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816200"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="65c9e-102">הסרת שירות הרקע עבור Microsoft Search ב-Bing</span><span class="sxs-lookup"><span data-stu-id="65c9e-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="65c9e-103">כדי להסיר את שירות הרקע עבור Microsoft Search ב-Bing, באפשרותך לנסות את התרופות הבאות:</span><span class="sxs-lookup"><span data-stu-id="65c9e-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="65c9e-104">כדי לחזור להגדרות מנוע החיפוש המקוריות, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="65c9e-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="65c9e-105">מ.</span><span class="sxs-lookup"><span data-stu-id="65c9e-105">a.</span></span> <span data-ttu-id="65c9e-106">החלף **[את](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) השימוש Bing כמנוע החיפוש המוגדר כברירת מחדל**.</span><span class="sxs-lookup"><span data-stu-id="65c9e-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="65c9e-107">b.</span><span class="sxs-lookup"><span data-stu-id="65c9e-107">b.</span></span> <span data-ttu-id="65c9e-108">[עבור אל מרכז הניהול של Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) ונקה את ההגדרה המשפיעה על כל המשתמשים בארגון שלך.</span><span class="sxs-lookup"><span data-stu-id="65c9e-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="65c9e-109">כדי להסיר את שירות הרקע ממכשיר בודד, בצע את המשימות הבאות:</span><span class="sxs-lookup"><span data-stu-id="65c9e-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="65c9e-110">מ.</span><span class="sxs-lookup"><span data-stu-id="65c9e-110">a.</span></span> <span data-ttu-id="65c9e-111">בחר **לוח הבקרה > תוכניות > תוכניות ותכונות**.</span><span class="sxs-lookup"><span data-stu-id="65c9e-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="65c9e-112">b.</span><span class="sxs-lookup"><span data-stu-id="65c9e-112">b.</span></span> <span data-ttu-id="65c9e-113">לחץ **באמצעות לחצן** העכבר הימני על Microsoft Search ב-Bing תחת רשימת התוכניות המותקנות ולאחר מכן לחץ על **הסר התקנה**.</span><span class="sxs-lookup"><span data-stu-id="65c9e-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="65c9e-114">כדי להסיר את שירות הרקע ממכשירים מרובים בארגון שלך, היכנס כמנהל מערכת והפעיל את הפקודה הבאה בקובץ script:</span><span class="sxs-lookup"><span data-stu-id="65c9e-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
