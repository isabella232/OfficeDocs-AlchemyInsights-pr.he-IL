---
title: פריסת Office 365 ProPlus עבור שימוש משותף ב-RDS, שרת מסופים או VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959461"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="371fa-102">פריסת Office 365 ProPlus עבור שימוש משותף ב-RDS, שרת מסופים או VDI</span><span class="sxs-lookup"><span data-stu-id="371fa-102">Deploying Office 365 ProPlus for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="371fa-103">כדי לפרוס את Office 365 ProPlus באמצעות שירותי שולחן עבודה מרוחק (RDS), שנקרא בעבר שירותי מסוף:</span><span class="sxs-lookup"><span data-stu-id="371fa-103">To deploy Office 365 ProPlus using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
- <span data-ttu-id="371fa-104">עליך להיות בעל 365 של Microsoft עבור תוכנית עסקית או תוכנית Office 365 הכוללת את Office 365 ProPlus, כגון Office 365 E3 או באמצעות הארגון E5.</span><span class="sxs-lookup"><span data-stu-id="371fa-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE] 
   > <span data-ttu-id="371fa-105">התוכניות של Office 365 Business ו-Office 365 Business Premium אינן כוללות את Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="371fa-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
- <span data-ttu-id="371fa-106">עליך להפוך [הפעלת מחשב משותפת](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)לזמינה.</span><span class="sxs-lookup"><span data-stu-id="371fa-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

> [!NOTE]
> <span data-ttu-id="371fa-107">באפשרותך גם להוריד ולהפעיל את [מסייע התמיכה והשחזור של Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) כדי להתקין את Office 365 proplus במצב משותף של הפעלת מחשב.</span><span class="sxs-lookup"><span data-stu-id="371fa-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>

<span data-ttu-id="371fa-108">לקבלת מידע נוסף אודות דרישות מוקדמות, הוראות התקנה והנחיות בנוגע להתקנות מותאמות אישית באמצעות כלי הפריסה של Office, ראה [פריסת office 365 ProPlus באמצעות שירותי שולחן עבודה מרוחק](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="371fa-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>

<span data-ttu-id="371fa-109">כדי לתקן שגיאות הקשורות להפעלת מחשב משותף:</span><span class="sxs-lookup"><span data-stu-id="371fa-109">To fix errors related to shared computer activation:</span></span>
- <span data-ttu-id="371fa-110">ראה [פתרון בעיות בהפעלת מחשב משותף עבור Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="371fa-110">See [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
- <span data-ttu-id="371fa-111">ראה [איפוס מצב ההפעלה של Office 365 ProPlus](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="371fa-111">See [Reset Office 365 ProPlus activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="371fa-112">אם ברצונך להתקין את Office 365 ProPlus ב-RDS ממרכז הניהול של Microsoft 365, ***המשתמש בהגדרות ברירת המחדל של ההתקנה***, השתמש בשלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="371fa-112">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1.  <span data-ttu-id="371fa-113">בדוק מה תוכנית Office 365 יש לך.</span><span class="sxs-lookup"><span data-stu-id="371fa-113">Check what Office 365 plan you have.</span></span> <span data-ttu-id="371fa-114">[למד כיצד לעשות זאת](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span><span class="sxs-lookup"><span data-stu-id="371fa-114">[Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2.  <span data-ttu-id="371fa-115">במקרה הצורך, עבור לתוכנית אחרת של Office 365.</span><span class="sxs-lookup"><span data-stu-id="371fa-115">If necessary, switch to a different Office 365 plan.</span></span> <span data-ttu-id="371fa-116">[למד כיצד לעשות זאת](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="371fa-116">[Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span></span>
3.  <span data-ttu-id="371fa-117">אם Office כבר מותקן בשרת RDS באמצעות כל תוכנית אחרת של Office 365, הסר את התקנתה.</span><span class="sxs-lookup"><span data-stu-id="371fa-117">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="371fa-118">לדוגמה, על-ידי הולך **ללוח** > **הבקרה הסר תוכנית**.</span><span class="sxs-lookup"><span data-stu-id="371fa-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="371fa-119">הסר [התקנה באמצעות מסייע התמיכה והשחזור של Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) אם אתה נתקל בבעיות.</span><span class="sxs-lookup"><span data-stu-id="371fa-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4.  <span data-ttu-id="371fa-120">בשרת RDS, היכנס למרכז הניהול של Microsoft 365 עם חשבון מנהל המערכת שלך [והתקן את Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="371fa-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5.  <span data-ttu-id="371fa-121">לאחר התקנת Office, ***אל תפתח או תיכנס*** ליישומי office כלשהם.</span><span class="sxs-lookup"><span data-stu-id="371fa-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6.  <span data-ttu-id="371fa-122">בשרת RDS, הפעל הפעלה משותפת של המחשב על-ידי עריכת הרישום על-ידי ביצוע השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="371fa-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="371fa-123">לחץ לחיצה ימנית על לחצן Windows בפינה השמאלית התחתונה של המסך ובחר באפשרות **הפעלה**.</span><span class="sxs-lookup"><span data-stu-id="371fa-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="371fa-124">בתיבה פתח את, הקלד **regedit**ולאחר מכן בחר **באפשרות אישור**.</span><span class="sxs-lookup"><span data-stu-id="371fa-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="371fa-125">בחר **כן** כאשר תתבקש לאפשר לעורך הרישום לבצע שינויים במכשיר.</span><span class="sxs-lookup"><span data-stu-id="371fa-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="371fa-126">בעורך הרישום, הוסף ערך מחרוזת של **רישוי שיתופיות** עם הגדרה של 1 תחת HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="371fa-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="371fa-127">בשרת RDS, ***היכנס כמשתמש קצה*** [וודא שהפעלת מחשב משותף זמינה עבור Office 365 proplus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="371fa-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

