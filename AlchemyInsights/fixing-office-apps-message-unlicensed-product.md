---
title: לא ניתן להפעיל את Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 9771a3244c5507312d43156525095fb9eaf7fa20
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812573"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="43a53-102">לא ניתן להפעיל את Office</span><span class="sxs-lookup"><span data-stu-id="43a53-102">Unable to activate Office</span></span>

- <span data-ttu-id="43a53-103">בדוק אם מצב המינוי שלך פג.</span><span class="sxs-lookup"><span data-stu-id="43a53-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="43a53-104">ודא שיש לך מנוי המאפשר רשיונות לקוח, כגון Office 365 Business או Business Premium, ו[ודא שלמשתמש הוקצה רשיון](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="43a53-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span></span>
- <span data-ttu-id="43a53-105">ודא שהמשתמש נכנס ל- Office באמצעות אותו החשבון שהוקצה לו רשיון.</span><span class="sxs-lookup"><span data-stu-id="43a53-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="43a53-106">בדוק את [דף תקינות השירות של Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) כדי לבדוק אם יש בעיות ידועות בשירות.</span><span class="sxs-lookup"><span data-stu-id="43a53-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="43a53-107">בדוק את חומת האש, תוכנת האנטי-וירוס והגדרות שרת ה- proxy כדי לוודא שהוא אינו חוסם את הגישה של יישומי Microsoft 365 לאינטרנט.</span><span class="sxs-lookup"><span data-stu-id="43a53-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="43a53-108">עיין ב[כתובות URL וטווחי כתובות IP של Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "כתובות URL וטווחי כתובות IP של Office 365").</span><span class="sxs-lookup"><span data-stu-id="43a53-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="43a53-109">**עצה** במחשבי Windows, אנו יכולים לאבחן ולפתור עבורך באופן אוטומטי כמה בעיות כניסה נפוצות של Office.</span><span class="sxs-lookup"><span data-stu-id="43a53-109">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="43a53-110">הורד והפעל את  **[מסייע התמיכה והשחזור של Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** כדי להשתמש בכלי האוטומטי שלנו.</span><span class="sxs-lookup"><span data-stu-id="43a53-110">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="43a53-111">השתמש בפעולות פתרון הבעיות הבאות:</span><span class="sxs-lookup"><span data-stu-id="43a53-111">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="43a53-112">פתח יישום של Office ו[צא](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) מחשבונות משתמשים קיימים.</span><span class="sxs-lookup"><span data-stu-id="43a53-112">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="43a53-113">[הסרה](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) ו[הקצה מחדש](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) רישיון Office ולאחר מכן [היכנס ל- Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) באמצעות חשבון המשתמש המושפע.</span><span class="sxs-lookup"><span data-stu-id="43a53-113">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="43a53-114">הפעל את ['פותר בעיות ההפעלה'](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="43a53-114">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="43a53-115">איפוס מצב ההפעלה של Office</span><span class="sxs-lookup"><span data-stu-id="43a53-115">Reset Office activation state</span></span>](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "איפוס מצב ההפעלה של Office")
- [<span data-ttu-id="43a53-116">בצע תיקון מקוון של Office</span><span class="sxs-lookup"><span data-stu-id="43a53-116">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="43a53-117">לפתרונות נוספים, ראה:</span><span class="sxs-lookup"><span data-stu-id="43a53-117">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="43a53-118">שגיאות מסוג "מוצר ללא רישיון" ושגיאות הפעלה ב- Office</span><span class="sxs-lookup"><span data-stu-id="43a53-118">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="43a53-119">השגיאה "מצטערים, אין לנו אפשרות להתחבר לחשבון שלך. נסה שוב במועד מאוחר יותר"בעת הפעלת Office</span><span class="sxs-lookup"><span data-stu-id="43a53-119">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)