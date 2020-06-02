---
title: התקנת משרד בשרת מסוף-לא מורשה
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: c781e9fd492ff97bc80667956e6609b3d40b28b4
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508629"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="0458a-102">התקנת Office בשרת מסופים</span><span class="sxs-lookup"><span data-stu-id="0458a-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="0458a-103">לפריסת יישומי Microsoft 365 עבור ארגון בשרת Windows באמצעות שירותי שולחן עבודה מרוחק (RDS), ששמו בעבר שירותי מסופים:</span><span class="sxs-lookup"><span data-stu-id="0458a-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="0458a-104">עליך לכלול מנוי של Microsoft 365 הכולל את Microsoft 365 Apps עבור ארגון, כגון Office 365 Enterprise E3 או Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="0458a-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="0458a-105">מיקרוסופט 365 Apps עבור עסקים ו-Microsoft 365 Apps עבור עסקים תוכניות פרימיום אינם כוללים Microsoft 365 Apps עבור הארגון.</span><span class="sxs-lookup"><span data-stu-id="0458a-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="0458a-106">עליך להפוך [הפעלת מחשב משותפת](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)לזמינה.</span><span class="sxs-lookup"><span data-stu-id="0458a-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="0458a-107">אם ברצונך להתקין את Microsoft 365 Apps עבור ארגון ב-RDS ממרכז הניהול של Microsoft 365, ***המשתמש בהגדרות ברירת המחדל של ההתקנה***, השתמש בשלבים הבאים.</span><span class="sxs-lookup"><span data-stu-id="0458a-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="0458a-108">באפשרותך גם להוריד ולהפעיל את [מסייע התמיכה והשחזור של microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) כדי להתקין את Microsoft 365 Apps עבור ארגון במצב הפעלה משותף של המחשב.</span><span class="sxs-lookup"><span data-stu-id="0458a-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="0458a-109">בדוק מה מנוי 365 של Microsoft שקיבלת.</span><span class="sxs-lookup"><span data-stu-id="0458a-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="0458a-110">למד כיצד</span><span class="sxs-lookup"><span data-stu-id="0458a-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="0458a-111">במקרה הצורך, עבור למנוי אחר של Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="0458a-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="0458a-112">למד כיצד</span><span class="sxs-lookup"><span data-stu-id="0458a-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="0458a-113">אם Office כבר מותקן בשרת ה-RDS באמצעות כל מנוי אחר של Microsoft 365, הסר את התקנתה.</span><span class="sxs-lookup"><span data-stu-id="0458a-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="0458a-114">לדוגמה, על-ידי הדרך ללוח \> הבקרה הסר תוכנית.</span><span class="sxs-lookup"><span data-stu-id="0458a-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="0458a-115">הסר [התקנה באמצעות מסייע התמיכה והשחזור של Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) אם אתה נתקל בבעיות.</span><span class="sxs-lookup"><span data-stu-id="0458a-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="0458a-116">בשרת RDS, היכנס למרכז הניהול של Microsoft 365 עם חשבון מנהל המערכת שלך [והתקן את microsoft 365 Apps עבור הארגון](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="0458a-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="0458a-117">לאחר התקנת Office, ***אל תפתח או תיכנס*** ליישומי office כלשהם.</span><span class="sxs-lookup"><span data-stu-id="0458a-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="0458a-118">בשרת RDS, הפעל הפעלה משותפת של המחשב על-ידי עריכת הרישום על-ידי ביצוע השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="0458a-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="0458a-119">לחץ לחיצה ימנית על לחצן Windows בפינה השמאלית התחתונה של המסך ובחר באפשרות הפעלה.</span><span class="sxs-lookup"><span data-stu-id="0458a-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="0458a-120">בתיבה פתח את, הקלד **regedit**ולאחר מכן בחר באישור.</span><span class="sxs-lookup"><span data-stu-id="0458a-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="0458a-121">בחר כן כאשר תתבקש לאפשר לעורך הרישום לבצע שינויים במכשיר.</span><span class="sxs-lookup"><span data-stu-id="0458a-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="0458a-122">בעורך הרישום, הוסף ערך מחרוזת של **רישוי שיתופיות** עם הגדרה של 1 תחת HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="0458a-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="0458a-123">בשרת RDS, ***היכנס כמשתמש קצה*** [וודא שהפעלת מחשב משותף מאופשרת עבור יישומי Microsoft 365 עבור הארגון](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="0458a-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="0458a-124">לקבלת פרטים נוספים על דרישות מוקדמות, הוראות התקנה והדרכה בהתקנות מותאמות אישית באמצעות כלי הפריסה של Office, עיין [בפריסת Microsoft 365 Apps לארגון באמצעות שירותי שולחן עבודה מרוחק](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="0458a-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="0458a-125">כדי לתקן שגיאות הקשורות להפעלת מחשב משותף, ראה [פתרון בעיות בהפעלה משותפת של מחשב עבור Microsoft 365 Apps עבור הארגון](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="0458a-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  