---
title: פתרון שגיאות מוצר ללא רשיון
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: bd2e8cb204edd7135fc34ef0d42ac8259434d37d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737954"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a><span data-ttu-id="a0f7b-102">הצעות לפתרון שגיאות "מוצר ללא רשיון"</span><span class="sxs-lookup"><span data-stu-id="a0f7b-102">Suggestions for solving "Unlicensed Product" errors</span></span>

<span data-ttu-id="a0f7b-103">כדי לפתור שגיאות אודות "מוצר ללא רשיון", נסה את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="a0f7b-103">To solve errors about an "Unlicensed Product," try the following:</span></span>

- <span data-ttu-id="a0f7b-104">בדוק אם תוקפו של מצב המנוי פג.</span><span class="sxs-lookup"><span data-stu-id="a0f7b-104">Check to see if your subscription status has expired.</span></span>
- <span data-ttu-id="a0f7b-105">ודא שיש לך מנוי המאפשר רשיונות לקוח, כגון יישומי Microsoft 365 for business או Business Premium, [וודא שהמשתמש הוקצה לו רשיון](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="a0f7b-105">Make sure you have a subscription that allows client licenses, such as Microsoft 365 Apps for business or Business Premium, and [ensure that the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> 
- <span data-ttu-id="a0f7b-106">ודא שהמשתמש כניסה ל-Office באמצעות אותו חשבון שהוקצה לו הרשיון.</span><span class="sxs-lookup"><span data-stu-id="a0f7b-106">Make sure the user is signing in to Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="a0f7b-107">בדוק את [דף תקינות השירות](https://docs.microsoft.com/office365/enterprise/view-service-health) כדי לבדוק אם קיימות בעיות ידועות בשירות.</span><span class="sxs-lookup"><span data-stu-id="a0f7b-107">Check the [Service health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="a0f7b-108">בדוק את חומת האש, תוכנת האנטי-וירוס והגדרות ה-proxy כדי לוודא שהם אינם חוסמים את הגישה לאינטרנט באפליקציות של Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a0f7b-108">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the Internet.</span></span> <span data-ttu-id="a0f7b-109">ראה [כתובות url וטווחי כתובות IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="a0f7b-109">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

<span data-ttu-id="a0f7b-110">ייתכן שתנסה גם את הפעולות הבאות לפתרון בעיות:</span><span class="sxs-lookup"><span data-stu-id="a0f7b-110">You may also try the following troubleshooting actions:</span></span> 

- <span data-ttu-id="a0f7b-111">פתח יישום של Office [וצא](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) מחשבונות משתמשים קיימים.</span><span class="sxs-lookup"><span data-stu-id="a0f7b-111">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="a0f7b-112">[הסר](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) [והקצה מחדש](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) את רשיון Office ולאחר מכן [היכנס ל-office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) באמצעות חשבון המשתמש המושפע.</span><span class="sxs-lookup"><span data-stu-id="a0f7b-112">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) the Office license, and then [sign in to Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="a0f7b-113">הפעלת [פותר בעיות ההפעלה](https://aka.ms/SARA-OfficeActivation-Alchemy).</span><span class="sxs-lookup"><span data-stu-id="a0f7b-113">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy).</span></span>
- <span data-ttu-id="a0f7b-114">[איפוס מצב ההפעלה של Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="a0f7b-114">[Reset the Office activation state](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span> 
- <span data-ttu-id="a0f7b-115">[ביצוע תיקון מקוון של Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span><span class="sxs-lookup"><span data-stu-id="a0f7b-115">[Perform an Online Repair of Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span></span>

<span data-ttu-id="a0f7b-116">לפתרונות נוספים, ראה:</span><span class="sxs-lookup"><span data-stu-id="a0f7b-116">For additional troubleshooting solutions, see:</span></span> 

- [<span data-ttu-id="a0f7b-117">שגיאות מסוג "מוצר ללא רישיון" ושגיאות הפעלה ב- Office</span><span class="sxs-lookup"><span data-stu-id="a0f7b-117">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [<span data-ttu-id="a0f7b-118">השגיאה "מצטערים, אין לנו אפשרות להתחבר לחשבון שלך. נסה שוב במועד מאוחר יותר"בעת הפעלת Office</span><span class="sxs-lookup"><span data-stu-id="a0f7b-118">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)