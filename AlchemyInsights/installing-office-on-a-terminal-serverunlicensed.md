---
title: התקנת office בשרת מסופים - ללא רשיון
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 6fc4bd5f6971ca833084a6a8ad6c25b3fdafb8dc
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35381730"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="e6b1b-102">התקנת Office בשרת מסופים</span><span class="sxs-lookup"><span data-stu-id="e6b1b-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="e6b1b-103">לפריסת Office 365 ProPlus בשרת Windows באמצעות שירותי שולחן עבודה מרוחק (RDS), לשעבר בשם שירותי מסופים:</span><span class="sxs-lookup"><span data-stu-id="e6b1b-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="e6b1b-104">דרושה לך תוכנית Office 365 הכוללת Office 365 ProPlus, כגון Office 365 ארגון E3 או ארגון E5.</span><span class="sxs-lookup"><span data-stu-id="e6b1b-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="e6b1b-105">תוכניות Office 365 עסקיים ו- Office 365 עסקיים איכותיים אינם כוללים ProPlus של Office 365.</span><span class="sxs-lookup"><span data-stu-id="e6b1b-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="e6b1b-106">עליך לאפשר [הפעלה במחשב משותף](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="e6b1b-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="e6b1b-107">אם ברצונך להתקין את Office 365 ProPlus RDS מתוך הפורטל Office 365, \* \* *המשתמשת הגדרות ברירת המחדל של ההתקנה* \* \*, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="e6b1b-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span>
  
1. <span data-ttu-id="e6b1b-108">בדוק איזו תוכנית Office 365 יש לך.</span><span class="sxs-lookup"><span data-stu-id="e6b1b-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="e6b1b-109">למד כיצד</span><span class="sxs-lookup"><span data-stu-id="e6b1b-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="e6b1b-110">אם מתכננים הצורך, מתג Office 365 שונים.</span><span class="sxs-lookup"><span data-stu-id="e6b1b-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="e6b1b-111">למד כיצד</span><span class="sxs-lookup"><span data-stu-id="e6b1b-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="e6b1b-112">אם כבר התקנת Office בשרת RDS באמצעות כל תוכניות אחרות של Office 365, הסר אותו.</span><span class="sxs-lookup"><span data-stu-id="e6b1b-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="e6b1b-113">לדוגמה, על-ידי מעבר אל לוח הבקרה \> להסיר התקנה של תוכנית.</span><span class="sxs-lookup"><span data-stu-id="e6b1b-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="e6b1b-114">הסרת התקנה באמצעות [התמיכה של Microsoft ומסייע שחזור](https://aka.ms/SARA-OfficeUninstall-Alchemy) אם אתה מפעיל לתוך בעיות.</span><span class="sxs-lookup"><span data-stu-id="e6b1b-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="e6b1b-115">בשרת RDS, היכנס אל פורטל Office 365 עם שלך חשבון מנהל המערכת ולהתקין את [Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="e6b1b-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="e6b1b-116">לאחר התקנת Office, \* \* *אין לפתוח או להיכנס* \* \* כל יישומי Office.</span><span class="sxs-lookup"><span data-stu-id="e6b1b-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span>

6. <span data-ttu-id="e6b1b-117">בשרת RDS, לאפשר הפעלה במחשב משותף על-ידי עריכת הרישום על-ידי ביצוע השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="e6b1b-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="e6b1b-118">לחץ לחיצה ימנית על לחצן Windows בפינה הימנית התחתונה של המסך, ובחר באפשרות הפעלה.</span><span class="sxs-lookup"><span data-stu-id="e6b1b-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="e6b1b-119">בתיבה פתח את, הקלד **regedit**ולאחר מכן לחץ על אישור.</span><span class="sxs-lookup"><span data-stu-id="e6b1b-119">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="e6b1b-120">בחר באפשרות כן כאשר תתבקש לאפשר בעורך הרישום כדי לבצע שינויים למכשיר שלך.</span><span class="sxs-lookup"><span data-stu-id="e6b1b-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="e6b1b-121">בעורך הרישום, הוסף ערך מחרוזת של **SharedComputerLicensing** עם הגדרה של 1 תחת HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="e6b1b-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="e6b1b-122">בשרת RDS, \* \* *היכנס בתור משתמש קצה* \* \*, [וודא כי הפעלת מחשב משותף זמין עבור Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="e6b1b-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="e6b1b-123">לקבלת פרטים נוספים על תנאים מוקדמים, הוראות ההתקנה והדרכה לגבי התקנות מותאמות אישית על-ידי שימוש בכלי הפריסה של Office, נא ראה [פריסת Office 365 ProPlus באמצעות שירותי שולחן עבודה מרוחק](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="e6b1b-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="e6b1b-124">כדי לתקן שגיאות הקשורות להפעלת מחשב משותף, נא ראה [פתרון בעיות עם הפעלת מחשב משותף עבור Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="e6b1b-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  