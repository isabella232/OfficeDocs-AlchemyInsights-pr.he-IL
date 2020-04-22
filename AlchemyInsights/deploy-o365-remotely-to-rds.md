---
title: פריסת מיקרוסופט 365 Apps עבור הארגון לשימוש משותף ב-RDS, שרת מסופים או VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: ddd44d40e9430ee31b8b734450dde0defef229d7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704706"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="d9deb-102">פריסת מיקרוסופט 365 Apps עבור הארגון לשימוש משותף ב-RDS, שרת מסופים או VDI</span><span class="sxs-lookup"><span data-stu-id="d9deb-102">Deploying Microsoft 365 Apps for enterprise for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="d9deb-103">כדי לפרוס את Microsoft 365 Apps עבור ארגון באמצעות שירותי שולחן עבודה מרוחק (RDS), שנקרא בעבר שירותי מסוף:</span><span class="sxs-lookup"><span data-stu-id="d9deb-103">To deploy Microsoft 365 Apps for enterprise using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
- <span data-ttu-id="d9deb-104">עליך להיות בעל 365 של Microsoft עבור תוכנית עסקית או תוכנית Office 365 הכוללת את Microsoft 365 Apps עבור הארגון, כגון Office 365 E3 או הארגון E5.</span><span class="sxs-lookup"><span data-stu-id="d9deb-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE] 
   > <span data-ttu-id="d9deb-105">התוכניות של Microsoft 365 לעסקים ו-Microsoft 365 Business Premium פרימיום לא כוללות את Microsoft 365 Apps עבור הארגון.</span><span class="sxs-lookup"><span data-stu-id="d9deb-105">The Microsoft 365 Apps for business and Microsoft 365 Business Premium Standard plans do not include Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="d9deb-106">עליך להפוך [הפעלת מחשב משותפת](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)לזמינה.</span><span class="sxs-lookup"><span data-stu-id="d9deb-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

> [!NOTE]
> <span data-ttu-id="d9deb-107">באפשרותך גם להוריד ולהפעיל את [מסייע התמיכה והשחזור של microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) כדי להתקין את Microsoft 365 Apps עבור ארגון במצב הפעלה משותף של המחשב.</span><span class="sxs-lookup"><span data-stu-id="d9deb-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>

<span data-ttu-id="d9deb-108">לקבלת מידע נוסף אודות דרישות מוקדמות, הוראות התקנה והנחיות בנוגע להתקנות מותאמות אישית באמצעות כלי הפריסה של Office, ראה [פריסה של Microsoft 365 Apps עבור ארגון באמצעות שירותי שולחן עבודה מרוחק](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="d9deb-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>

<span data-ttu-id="d9deb-109">כדי לתקן שגיאות הקשורות להפעלת מחשב משותף:</span><span class="sxs-lookup"><span data-stu-id="d9deb-109">To fix errors related to shared computer activation:</span></span>
- <span data-ttu-id="d9deb-110">ראה [פתרון בעיות בהפעלת מחשב משותף עבור Microsoft 365 Apps עבור הארגון](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="d9deb-110">See [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
- <span data-ttu-id="d9deb-111">ראה [איפוס יישומי Microsoft 365 עבור מצב הפעלה ארגונית](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="d9deb-111">See [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="d9deb-112">אם ברצונך להתקין את Microsoft 365 Apps עבור ארגון ב-RDS ממרכז הניהול של Microsoft 365, ***המשתמש בהגדרות ברירת המחדל של ההתקנה***, השתמש בשלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="d9deb-112">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1.    <span data-ttu-id="d9deb-113">בדוק איזה מנוי יש לך.</span><span class="sxs-lookup"><span data-stu-id="d9deb-113">Check what subscription you have.</span></span> <span data-ttu-id="d9deb-114">[למד כיצד לעשות זאת](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span><span class="sxs-lookup"><span data-stu-id="d9deb-114">[Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2.    <span data-ttu-id="d9deb-115">במידת הצורך, עבור למנוי אחר.</span><span class="sxs-lookup"><span data-stu-id="d9deb-115">If necessary, switch to a different subscription.</span></span> <span data-ttu-id="d9deb-116">[למד כיצד לעשות זאת](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="d9deb-116">[Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span></span>
3.    <span data-ttu-id="d9deb-117">אם Office כבר מותקן בשרת ה-RDS באמצעות כל מנוי אחר של Microsoft, הסר את התקנתה.</span><span class="sxs-lookup"><span data-stu-id="d9deb-117">If Office is already installed on the RDS server using any other Microsoft subscriptions, uninstall it.</span></span> <span data-ttu-id="d9deb-118">לדוגמה, על-ידי הולך **ללוח** > **הבקרה הסר תוכנית**.</span><span class="sxs-lookup"><span data-stu-id="d9deb-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="d9deb-119">הסר [התקנה באמצעות מסייע התמיכה והשחזור של Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) אם אתה נתקל בבעיות.</span><span class="sxs-lookup"><span data-stu-id="d9deb-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4.    <span data-ttu-id="d9deb-120">בשרת RDS, היכנס למרכז הניהול של Microsoft 365 עם חשבון מנהל המערכת שלך [והתקן את microsoft 365 Apps עבור הארגון](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="d9deb-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5.    <span data-ttu-id="d9deb-121">לאחר התקנת Office, ***אל תפתח או תיכנס*** ליישומי office כלשהם.</span><span class="sxs-lookup"><span data-stu-id="d9deb-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6.    <span data-ttu-id="d9deb-122">בשרת RDS, הפעל הפעלה משותפת של המחשב על-ידי עריכת הרישום על-ידי ביצוע השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="d9deb-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="d9deb-123">לחץ לחיצה ימנית על לחצן Windows בפינה השמאלית התחתונה של המסך ובחר באפשרות **הפעלה**.</span><span class="sxs-lookup"><span data-stu-id="d9deb-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="d9deb-124">בתיבה פתח את, הקלד **regedit**ולאחר מכן בחר **באפשרות אישור**.</span><span class="sxs-lookup"><span data-stu-id="d9deb-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="d9deb-125">בחר **כן** כאשר תתבקש לאפשר לעורך הרישום לבצע שינויים במכשיר.</span><span class="sxs-lookup"><span data-stu-id="d9deb-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="d9deb-126">בעורך הרישום, הוסף ערך מחרוזת של **רישוי שיתופיות** עם הגדרה של 1 תחת HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="d9deb-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="d9deb-127">בשרת RDS, ***היכנס כמשתמש קצה*** [וודא שהפעלת מחשב משותף מאופשרת עבור יישומי Microsoft 365 עבור הארגון](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="d9deb-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

