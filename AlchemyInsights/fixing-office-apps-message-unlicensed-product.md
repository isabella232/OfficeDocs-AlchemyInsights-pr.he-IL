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
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798681"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="5cf15-102">לא ניתן להפעיל את Office</span><span class="sxs-lookup"><span data-stu-id="5cf15-102">Unable to activate Office</span></span>

<span data-ttu-id="5cf15-103">**הערה**: אם אתה משתמש בגירסה קודמת של Windows (לדוגמה, Windows 7), ודא ש- TLS 1.2 זמין כברירת המחדל.</span><span class="sxs-lookup"><span data-stu-id="5cf15-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="5cf15-104">לקבלת מידע נוסף, ראה [עדכון כדי להפוך את TLS 1.1 ו- TLS 1.2 לזמינים](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)כפרוטוקולים מאובטחים המהווים ברירת מחדל ב- WinHTTP ב- Windows.</span><span class="sxs-lookup"><span data-stu-id="5cf15-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="5cf15-105">בדוק אם מצב המינוי שלך פג.</span><span class="sxs-lookup"><span data-stu-id="5cf15-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="5cf15-106">ודא שיש לך מנוי המאפשר רשיונות לקוח, כגון Office 365 Business או Business Premium, ו[ודא שלמשתמש הוקצה רשיון](/microsoft-365/admin/manage/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="5cf15-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="5cf15-107">ודא שהמשתמש נכנס ל- Office באמצעות אותו החשבון שהוקצה לו רשיון.</span><span class="sxs-lookup"><span data-stu-id="5cf15-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="5cf15-108">בדוק את [דף תקינות השירות של Office 365](/office365/enterprise/view-service-health) כדי לבדוק אם יש בעיות ידועות בשירות.</span><span class="sxs-lookup"><span data-stu-id="5cf15-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="5cf15-109">בדוק את חומת האש, תוכנת האנטי-וירוס והגדרות שרת ה- proxy כדי לוודא שהוא אינו חוסם את הגישה של יישומי Microsoft 365 לאינטרנט.</span><span class="sxs-lookup"><span data-stu-id="5cf15-109">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="5cf15-110">עיין ב[כתובות URL וטווחי כתובות IP של Office 365](/office365/enterprise/urls-and-ip-address-ranges "כתובות URL וטווחי כתובות IP של Office 365").</span><span class="sxs-lookup"><span data-stu-id="5cf15-110">Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="5cf15-111">**עצה** במחשבי Windows, אנו יכולים לאבחן ולפתור עבורך באופן אוטומטי כמה בעיות כניסה נפוצות של Office.</span><span class="sxs-lookup"><span data-stu-id="5cf15-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="5cf15-112">הורד והפעל את  **[מסייע התמיכה והשחזור של Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** כדי להשתמש בכלי האוטומטי שלנו.</span><span class="sxs-lookup"><span data-stu-id="5cf15-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="5cf15-113">השתמש בפעולות פתרון הבעיות הבאות:</span><span class="sxs-lookup"><span data-stu-id="5cf15-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="5cf15-114">פתח יישום של Office ו[צא](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) מחשבונות משתמשים קיימים.</span><span class="sxs-lookup"><span data-stu-id="5cf15-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="5cf15-115">[הסרה](/microsoft-365/admin/manage/remove-licenses-from-users) ו[הקצה מחדש](/microsoft-365/admin/manage/assign-licenses-to-users) רישיון Office ולאחר מכן [היכנס ל- Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) באמצעות חשבון המשתמש המושפע.</span><span class="sxs-lookup"><span data-stu-id="5cf15-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="5cf15-116">הפעל את ['פותר בעיות ההפעלה'](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="5cf15-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="5cf15-117">איפוס מצב ההפעלה של Office</span><span class="sxs-lookup"><span data-stu-id="5cf15-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "איפוס מצב ההפעלה של Office")
- [<span data-ttu-id="5cf15-118">בצע תיקון מקוון של Office</span><span class="sxs-lookup"><span data-stu-id="5cf15-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="5cf15-119">לפתרונות נוספים, ראה:</span><span class="sxs-lookup"><span data-stu-id="5cf15-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="5cf15-120">שגיאות מסוג "מוצר ללא רישיון" ושגיאות הפעלה ב- Office</span><span class="sxs-lookup"><span data-stu-id="5cf15-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="5cf15-121">השגיאה "מצטערים, אין לנו אפשרות להתחבר לחשבון שלך. נסה שוב במועד מאוחר יותר"בעת הפעלת Office</span><span class="sxs-lookup"><span data-stu-id="5cf15-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)