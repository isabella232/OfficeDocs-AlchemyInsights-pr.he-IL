---
title: פריסת יישומי Microsoft 365 עבור enterprise לשימוש משותף ב-RDS, Terminal Server או VDI
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
- "9001419"
- "3411"
ms.openlocfilehash: bd30d99221e3ddd0b07db0db78009f346babd2d0
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786278"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="530c7-102">פריסת יישומי Microsoft 365 עבור enterprise לשימוש משותף ב-RDS, Terminal Server או VDI</span><span class="sxs-lookup"><span data-stu-id="530c7-102">Deploying Microsoft 365 Apps for enterprise for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="530c7-103">כדי לפרוס את יישומי Microsoft 365 עבור enterprise באמצעות שירותי שולחן עבודה מרוחק (RDS), שנקראו בעבר ' שירותי מסוף ':</span><span class="sxs-lookup"><span data-stu-id="530c7-103">To deploy Microsoft 365 Apps for enterprise using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
- <span data-ttu-id="530c7-104">דרושה לך תוכנית Microsoft 365 For Business או תוכנית של Office 365 הכוללת אפליקציות של Microsoft 365 לארגונים, כגון Office 365 Enterprise E3 או Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="530c7-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE] 
   > <span data-ttu-id="530c7-105">התוכניות הסטנדרטיות של microsoft 365 לעסקים ו-Microsoft 365 Business Premium אינן כוללות יישומי Microsoft 365 עבור enterprise.</span><span class="sxs-lookup"><span data-stu-id="530c7-105">The Microsoft 365 Apps for business and Microsoft 365 Business Premium Standard plans do not include Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="530c7-106">עליך להפוך [הפעלת מחשב משותפת](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)לזמינה.</span><span class="sxs-lookup"><span data-stu-id="530c7-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

> [!NOTE]
> <span data-ttu-id="530c7-107">באפשרותך גם להוריד ולהפעיל את [מסייע התמיכה והשחזור של microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) כדי להתקין את יישומי microsoft 365 for enterprise במצב הפעלה משותפת של מחשב.</span><span class="sxs-lookup"><span data-stu-id="530c7-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>

<span data-ttu-id="530c7-108">לקבלת מידע נוסף אודות דרישות מוקדמות, הוראות הגדרה והנחיות לגבי התקנות מותאמות אישית באמצעות כלי הפריסה של Office, ראה [פריסת יישומי Microsoft 365 עבור enterprise באמצעות שירותי שולחן עבודה מרוחק](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="530c7-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>

<span data-ttu-id="530c7-109">כדי לתקן שגיאות הקשורות להפעלת מחשב משותפת:</span><span class="sxs-lookup"><span data-stu-id="530c7-109">To fix errors related to shared computer activation:</span></span>
- <span data-ttu-id="530c7-110">ראה [פתרון בעיות בהפעלת מחשב משותף עבור יישומי Microsoft 365 עבור enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="530c7-110">See [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
- <span data-ttu-id="530c7-111">ראה [איפוס יישומי Microsoft 365 עבור מצב הפעלה ארגונית](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="530c7-111">See [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="530c7-112">אם ברצונך להתקין את יישומי Microsoft 365 עבור enterprise ב-RDS מתוך מרכז הניהול של Microsoft 365, ***המשתמש בהגדרות ההתקנה המשמשות כברירת מחדל***, השתמש בשלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="530c7-112">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1.    <span data-ttu-id="530c7-113">בדוק איזה מנוי יש לך.</span><span class="sxs-lookup"><span data-stu-id="530c7-113">Check what subscription you have.</span></span> <span data-ttu-id="530c7-114">[למד כיצד לעשות זאת](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span><span class="sxs-lookup"><span data-stu-id="530c7-114">[Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2.    <span data-ttu-id="530c7-115">במידת הצורך, עבור למנוי אחר.</span><span class="sxs-lookup"><span data-stu-id="530c7-115">If necessary, switch to a different subscription.</span></span> <span data-ttu-id="530c7-116">[למד כיצד לעשות זאת](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="530c7-116">[Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span></span>
3.    <span data-ttu-id="530c7-117">אם Office כבר מותקן בשרת RDS באמצעות מנויים אחרים של Microsoft, הסר את התקנתו.</span><span class="sxs-lookup"><span data-stu-id="530c7-117">If Office is already installed on the RDS server using any other Microsoft subscriptions, uninstall it.</span></span> <span data-ttu-id="530c7-118">לדוגמה, על-ידי מעבר אל **'**  >  **הסרת התקנה של תוכנית ' בלוח הבקרה**.</span><span class="sxs-lookup"><span data-stu-id="530c7-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="530c7-119">הסר התקנה באמצעות [מסייע התמיכה והשחזור של Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) אם אתה נתקל בבעיות.</span><span class="sxs-lookup"><span data-stu-id="530c7-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4.    <span data-ttu-id="530c7-120">בשרת RDS, היכנס למרכז הניהול של Microsoft 365 עם חשבון מנהל המערכת שלך [והתקן את יישומי microsoft 365 עבור הארגון](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="530c7-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5.    <span data-ttu-id="530c7-121">לאחר התקנת Office, ***אל תפתח או תיכנס*** ליישומי Office כלשהם.</span><span class="sxs-lookup"><span data-stu-id="530c7-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6.    <span data-ttu-id="530c7-122">בשרת RDS, אפשר הפעלת מחשב משותפת על-ידי עריכת הרישום על-ידי ביצוע השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="530c7-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="530c7-123">לחץ באמצעות לחצן העכבר הימני על לחצן Windows בפינה הימנית התחתונה של המסך ובחר **הרצה**.</span><span class="sxs-lookup"><span data-stu-id="530c7-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="530c7-124">בתיבה פתח, הקלד **regedit**ולאחר מכן בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="530c7-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="530c7-125">בחר **כן** כאשר תתבקש לאפשר לעורך הרישום לבצע שינויים במכשיר שלך.</span><span class="sxs-lookup"><span data-stu-id="530c7-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="530c7-126">בעורך הרישום, הוסף ערך מחרוזת של **SharedComputerLicensing** עם הגדרה של 1 תחת HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="530c7-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="530c7-127">בשרת RDS, ***היכנס כמשתמש קצה*** [וודא שהפעלת מחשב משותפת זמינה עבור יישומי Microsoft 365 for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="530c7-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

