---
title: פתרון בעיות בסינכרון סיסמאות
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664927"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="0a5b7-102">פתרון בעיות בסינכרון סיסמאות</span><span class="sxs-lookup"><span data-stu-id="0a5b7-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="0a5b7-103">כדי לפתור בעיות בסינכרון סיסמאות, התחל באמצעות משימת התחברות זו לפתרון בעיות כדי לקבוע מדוע סיסמאות אינן מסונכרנות.</span><span class="sxs-lookup"><span data-stu-id="0a5b7-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="0a5b7-104">כדי להתחיל, עבור אל [ניהול סינכרון ישיר](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="0a5b7-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="0a5b7-105">פתח הפעלה חדשה של Windows PowerShell בשרת החיבור של תכלת לספירה ובחר באפשרות **הפעל כמנהל** .</span><span class="sxs-lookup"><span data-stu-id="0a5b7-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="0a5b7-106">הפעיל את Set-ExecutionPolicy RemoteSigned או Set-ExecutionPolicy בלתי מוגבל.</span><span class="sxs-lookup"><span data-stu-id="0a5b7-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="0a5b7-107">הפעל את אשף ההתחברות של תכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="0a5b7-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="0a5b7-108">עבור אל דף המשימות הנוספות > **פתור את הבעיות**  >  **הבאות**.</span><span class="sxs-lookup"><span data-stu-id="0a5b7-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="0a5b7-109">בחר **הפעל** כדי לפתוח את תפריט פתרון בעיות של PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0a5b7-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="0a5b7-110">בחר באפשרות **פתרון בעיות בסינכרון סיסמאות**.</span><span class="sxs-lookup"><span data-stu-id="0a5b7-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="0a5b7-111">הבעיה היא בדרך כלל שסיסמה אינה מסונכרנת עבור חשבון משתמש ספציפי.</span><span class="sxs-lookup"><span data-stu-id="0a5b7-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="0a5b7-112">**הערות** סינכרון סיסמאות נכשל אם סינכרון הסיסמאות האחרון שהצליח היה לפני זמן מה.</span><span class="sxs-lookup"><span data-stu-id="0a5b7-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="0a5b7-113">לקבלת עזרה נוספת בפתרון בעיות בסינכרון סיסמאות, ראה [פתרון בעיות בסינכרון hash של סיסמאות באמצעות הסינכרון של תכלת AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="0a5b7-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>