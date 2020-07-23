---
title: פתרון בעיות בסנכרון סיסמאות
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387878"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="cb7a6-102">פתרון בעיות בסנכרון סיסמאות</span><span class="sxs-lookup"><span data-stu-id="cb7a6-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="cb7a6-103">כדי לפתור בעיות בסינכרון הסיסמאות, התחל בשימוש במשימה זו של פתרון בעיות של התחברות אד-משתמשים כדי לקבוע מדוע סיסמאות אינן מסינכרון.</span><span class="sxs-lookup"><span data-stu-id="cb7a6-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="cb7a6-104">כדי להתחיל, עבור [לניהול סינכרון ישיר](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="cb7a6-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="cb7a6-105">פתח הפעלה חדשה של Windows PowerShell בשרת החיבור של תכלת AD שלך, ובחר באפשרות **הפעל כמנהל** .</span><span class="sxs-lookup"><span data-stu-id="cb7a6-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="cb7a6-106">הפעלה של מדיניות הגדרת המדיניות חתומה או הוגדרה מדיניות לא מוגבלת.</span><span class="sxs-lookup"><span data-stu-id="cb7a6-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="cb7a6-107">הפעל את אשף התקשרות תכלת.</span><span class="sxs-lookup"><span data-stu-id="cb7a6-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="cb7a6-108">עבור אל דף הפעילויות הנוספות _ gt_ **פתור**את הפעולות  >  **הבאות**.</span><span class="sxs-lookup"><span data-stu-id="cb7a6-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="cb7a6-109">בחר באפשרות ' **הפעלה** ' כדי לפתוח את תפריט פתרון בעיות PowerShell.</span><span class="sxs-lookup"><span data-stu-id="cb7a6-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="cb7a6-110">בחר **בפתרון בעיות בסינכרון סיסמאות**.</span><span class="sxs-lookup"><span data-stu-id="cb7a6-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="cb7a6-111">הבעיה היא בדרך כלל שסיסמה אינה מסונכרנת עבור חשבון משתמש מסוים.</span><span class="sxs-lookup"><span data-stu-id="cb7a6-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="cb7a6-112">**פתקים** סינכרון הסיסמה נכשל אם סינכרון הסיסמה המוצלח האחרון היה לפני זמן מה.</span><span class="sxs-lookup"><span data-stu-id="cb7a6-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="cb7a6-113">לקבלת עזרה נוספת לפתרון בעיות בסינכרון סיסמאות, ראה [פתרון בעיות בסינכרון hash של סיסמה עם סינכרון התקשרות תכלת](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="cb7a6-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>