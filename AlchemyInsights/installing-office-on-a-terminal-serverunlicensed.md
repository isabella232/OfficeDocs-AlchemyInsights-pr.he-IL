---
title: התקנת משרד בשרת מסוף-לא מורשה
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
ms.openlocfilehash: 53071224a7c33532d864cd70b84bf0e3cc6a992f
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36735390"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="a8234-102">התקנת Office בשרת מסופים</span><span class="sxs-lookup"><span data-stu-id="a8234-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="a8234-103">עבור פריסת Office 365 ProPlus בשרת Windows באמצעות שירותי שולחן עבודה מרוחק (RDS), שנקרא בעבר שירותי מסוף:</span><span class="sxs-lookup"><span data-stu-id="a8234-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="a8234-104">דרושה לך תוכנית Office 365 הכוללת את Office 365 ProPlus, כגון Office 365 Enterprise E3 או Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="a8234-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="a8234-105">התוכניות של Office 365 Business ו-Office 365 Business Premium אינן כוללות את Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="a8234-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="a8234-106">עליך להפוך [הפעלת מחשב משותפת](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)לזמינה.</span><span class="sxs-lookup"><span data-stu-id="a8234-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="a8234-107">אם ברצונך להתקין את Office 365 ProPlus ב-RDS ממרכז הניהול של Microsoft 365, ***המשתמש בהגדרות ברירת המחדל של ההתקנה***, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="a8234-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, follow these steps:</span></span>
  
1. <span data-ttu-id="a8234-108">בדוק מה תוכנית Office 365 יש לך.</span><span class="sxs-lookup"><span data-stu-id="a8234-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="a8234-109">למד כיצד</span><span class="sxs-lookup"><span data-stu-id="a8234-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="a8234-110">במקרה הצורך, עבור לתוכנית אחרת של Office 365.</span><span class="sxs-lookup"><span data-stu-id="a8234-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="a8234-111">למד כיצד</span><span class="sxs-lookup"><span data-stu-id="a8234-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="a8234-112">אם Office כבר מותקן בשרת RDS באמצעות כל תוכנית אחרת של Office 365, הסר את התקנתה.</span><span class="sxs-lookup"><span data-stu-id="a8234-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="a8234-113">לדוגמה, על-ידי הדרך \> ללוח הבקרה הסר תוכנית.</span><span class="sxs-lookup"><span data-stu-id="a8234-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="a8234-114">הסר [התקנה באמצעות מסייע התמיכה והשחזור של Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) אם אתה נתקל בבעיות.</span><span class="sxs-lookup"><span data-stu-id="a8234-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="a8234-115">בשרת RDS, היכנס למרכז הניהול של Microsoft 365 עם חשבון מנהל המערכת שלך [והתקן את Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="a8234-115">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="a8234-116">לאחר התקנת Office, ***אל תפתח או תיכנס*** ליישומי office כלשהם.</span><span class="sxs-lookup"><span data-stu-id="a8234-116">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="a8234-117">בשרת RDS, הפעל הפעלה משותפת של המחשב על-ידי עריכת הרישום על-ידי ביצוע השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="a8234-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="a8234-118">לחץ לחיצה ימנית על לחצן Windows בפינה השמאלית התחתונה של המסך ובחר באפשרות הפעלה.</span><span class="sxs-lookup"><span data-stu-id="a8234-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="a8234-119">בתיבה פתח את, הקלד **regedit**ולאחר מכן בחר באישור.</span><span class="sxs-lookup"><span data-stu-id="a8234-119">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="a8234-120">בחר כן כאשר תתבקש לאפשר לעורך הרישום לבצע שינויים במכשיר.</span><span class="sxs-lookup"><span data-stu-id="a8234-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="a8234-121">בעורך הרישום, הוסף ערך מחרוזת של **רישוי שיתופיות** עם הגדרה של 1 תחת HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="a8234-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="a8234-122">בשרת RDS, ***היכנס כמשתמש קצה*** [וודא שהפעלת מחשב משותף זמינה עבור Office 365 proplus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="a8234-122">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="a8234-123">לקבלת פרטים נוספים על דרישות מוקדמות, הוראות התקנה והדרכה בהתקנות מותאמות אישית באמצעות כלי הפריסה של Office, עיין [בפריסת office 365 ProPlus באמצעות שירותי שולחן עבודה מרוחק](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="a8234-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="a8234-124">כדי לתקן שגיאות הקשורות להפעלת מחשב משותף, ראה [פתרון בעיות עם הפעלת מחשב משותף עבור Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="a8234-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  