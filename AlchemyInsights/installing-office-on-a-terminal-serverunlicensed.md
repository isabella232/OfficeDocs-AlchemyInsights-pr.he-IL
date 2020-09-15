---
title: התקנת office בשרת מסוף-לא מורשה
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663118"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="247ab-102">התקנת Office בשרת מסופים</span><span class="sxs-lookup"><span data-stu-id="247ab-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="247ab-103">לפריסת יישומי Microsoft 365 עבור enterprise בשרת Windows באמצעות שירותי שולחן עבודה מרוחק (RDS), שנקראו בעבר ' שירותי מסוף ':</span><span class="sxs-lookup"><span data-stu-id="247ab-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="247ab-104">דרוש לך מנוי של Microsoft 365 הכולל יישומי Microsoft 365 עבור enterprise, כגון Office 365 Enterprise E3 או Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="247ab-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="247ab-105">האפליקציות של Microsoft 365 לעסקים ו-Microsoft 365 Apps עבור business Premium אינן כוללות אפליקציות של Microsoft 365 עבור enterprise.</span><span class="sxs-lookup"><span data-stu-id="247ab-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="247ab-106">עליך להפוך [הפעלת מחשב משותפת](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)לזמינה.</span><span class="sxs-lookup"><span data-stu-id="247ab-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="247ab-107">אם ברצונך להתקין את יישומי Microsoft 365 עבור enterprise ב-RDS מתוך מרכז הניהול של Microsoft 365, ***המשתמש בהגדרות ברירת המחדל של ההתקנה***, השתמש בשלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="247ab-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="247ab-108">באפשרותך גם להוריד ולהפעיל את [מסייע התמיכה והשחזור של microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) כדי להתקין את יישומי microsoft 365 for enterprise במצב הפעלה משותפת של מחשב.</span><span class="sxs-lookup"><span data-stu-id="247ab-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="247ab-109">בדוק את מנוי Microsoft 365 שברשותך.</span><span class="sxs-lookup"><span data-stu-id="247ab-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="247ab-110">למד כיצד</span><span class="sxs-lookup"><span data-stu-id="247ab-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="247ab-111">במידת הצורך, עבור למנוי אחר של Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="247ab-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="247ab-112">למד כיצד</span><span class="sxs-lookup"><span data-stu-id="247ab-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="247ab-113">אם Office כבר מותקן בשרת RDS באמצעות מנויים אחרים של Microsoft 365, הסר את התקנתו.</span><span class="sxs-lookup"><span data-stu-id="247ab-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="247ab-114">לדוגמה, על-ידי מעבר אל ' \> הסרת התקנה של תוכנית ' בלוח הבקרה.</span><span class="sxs-lookup"><span data-stu-id="247ab-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="247ab-115">הסר התקנה באמצעות [מסייע התמיכה והשחזור של Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) אם אתה נתקל בבעיות.</span><span class="sxs-lookup"><span data-stu-id="247ab-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="247ab-116">בשרת RDS, היכנס למרכז הניהול של Microsoft 365 עם חשבון מנהל המערכת שלך [והתקן את יישומי microsoft 365 עבור הארגון](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="247ab-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="247ab-117">לאחר התקנת Office, ***אל תפתח או תיכנס*** ליישומי Office כלשהם.</span><span class="sxs-lookup"><span data-stu-id="247ab-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="247ab-118">בשרת RDS, אפשר הפעלת מחשב משותפת על-ידי עריכת הרישום על-ידי ביצוע השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="247ab-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="247ab-119">לחץ באמצעות לחצן העכבר הימני על לחצן Windows בפינה הימנית התחתונה של המסך ובחר הרצה.</span><span class="sxs-lookup"><span data-stu-id="247ab-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="247ab-120">בתיבה פתח, הקלד **regedit**ולאחר מכן בחר אישור.</span><span class="sxs-lookup"><span data-stu-id="247ab-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="247ab-121">בחר כן כאשר תתבקש לאפשר לעורך הרישום לבצע שינויים במכשיר שלך.</span><span class="sxs-lookup"><span data-stu-id="247ab-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="247ab-122">בעורך הרישום, הוסף ערך מחרוזת של **SharedComputerLicensing** עם הגדרה של 1 תחת HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="247ab-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="247ab-123">בשרת RDS, ***היכנס כמשתמש קצה*** [וודא שהפעלת מחשב משותפת זמינה עבור יישומי Microsoft 365 for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="247ab-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="247ab-124">לקבלת פרטים נוספים על דרישות מוקדמות, הוראות הגדרה והנחיות לגבי התקנות מותאמות אישית באמצעות כלי הפריסה של Office, ראה [פריסת יישומי Microsoft 365 עבור enterprise באמצעות שירותי שולחן עבודה מרוחק](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="247ab-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="247ab-125">כדי לתקן שגיאות הקשורות להפעלת מחשב משותף, ראה [פתרון בעיות בהפעלת מחשב משותפת עבור יישומי Microsoft 365 עבור enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="247ab-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  