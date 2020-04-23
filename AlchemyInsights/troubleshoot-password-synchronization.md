---
title: פתרון בעיות בסנכרון סיסמאות
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732511"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="a3ae2-102">פתרון בעיות בסנכרון סיסמאות</span><span class="sxs-lookup"><span data-stu-id="a3ae2-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="a3ae2-103">כדי לפתור בעיות שבהן לא מסונכרנים סיסמאות עם הגירסה 1.1.614.0 או גירסאות מאוחרות יותר של התכונה:</span><span class="sxs-lookup"><span data-stu-id="a3ae2-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="a3ae2-104">פתח הפעלה חדשה של Windows PowerShell בשרת החיבור שלך בתכלת AD עם **הפעלת האפשרות מנהל** .</span><span class="sxs-lookup"><span data-stu-id="a3ae2-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="a3ae2-105">הפעלה של **מדיניות הגדרת המדיניות חתומה** או **מוגדרת על-ידי מדיניות בלתי מוגבלת**.</span><span class="sxs-lookup"><span data-stu-id="a3ae2-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="a3ae2-106">הפעל את אשף התקשרות תכלת.</span><span class="sxs-lookup"><span data-stu-id="a3ae2-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="a3ae2-107">נווט לדף **פעילויות נוספות** , בחר **בפתרון בעיות**ולחץ על **הבא**.</span><span class="sxs-lookup"><span data-stu-id="a3ae2-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="a3ae2-108">בדף פתרון בעיות, לחץ על **הפעלה כדי להפעיל את תפריט פתרון התקלות** ב-PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a3ae2-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="a3ae2-109">בתפריט הראשי, בחר **בפתרון בעיות בסינכרון סיסמאות**.</span><span class="sxs-lookup"><span data-stu-id="a3ae2-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="a3ae2-110">בתפריט המשנה, בחר באפשרות **סינכרון סיסמה אינו פועל כלל**.</span><span class="sxs-lookup"><span data-stu-id="a3ae2-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="a3ae2-111">**הכרת התוצאות של משימת פתרון התקלות**</span><span class="sxs-lookup"><span data-stu-id="a3ae2-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="a3ae2-112">משימת פתרון התקלות מבצעת את הבדיקות הבאות:</span><span class="sxs-lookup"><span data-stu-id="a3ae2-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="a3ae2-113">מאמת שתכונת סינכרון הסיסמאות מאופשרת עבור דייר ה-"תכלת לספירה" שלך.</span><span class="sxs-lookup"><span data-stu-id="a3ae2-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="a3ae2-114">מאמת כי שרת החיבור של תכלת AD אינו במצב אחסון זמני.</span><span class="sxs-lookup"><span data-stu-id="a3ae2-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="a3ae2-115">עבור כל מחבר פעיל מקומי של Active Directory (התואם ליער Active Directory קיים):</span><span class="sxs-lookup"><span data-stu-id="a3ae2-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="a3ae2-116">אימות שתכונת סינכרון הסיסמאות מאופשרת.</span><span class="sxs-lookup"><span data-stu-id="a3ae2-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="a3ae2-117">מחפש אירועי פעימה של סינכרון סיסמאות ביומני האירועים של יישום Windows.</span><span class="sxs-lookup"><span data-stu-id="a3ae2-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="a3ae2-118">עבור כל קבוצת מחשבים של Active Directory תחת המחבר Active Directory המקומי:</span><span class="sxs-lookup"><span data-stu-id="a3ae2-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="a3ae2-119">מאמת שניתן להגיע לתחום משרת החיבור של תכלת.</span><span class="sxs-lookup"><span data-stu-id="a3ae2-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="a3ae2-120">מאמת שלחשבונות המשמשים את שירותי התחום של Active Directory (AD DS) שבשימוש מחבר הספריה המקומי יש את שם המשתמש, הסיסמה וההרשאות הדרושים לסנכרון סיסמאות.</span><span class="sxs-lookup"><span data-stu-id="a3ae2-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="a3ae2-121">לקבלת עזרה נוספת לפתרון בעיות בסינכרון הסיסמה, ראה [פתרון בעיות בסינכרון סיסמאות באמצעות סינכרון התקשרות תכלת](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="a3ae2-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  