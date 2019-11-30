---
title: סוגיית ההפעלה-אין באפשרותנו להתחבר כרגע
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628243"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="ba337-102">תיקון האפליקציות של Office "אנחנו לא יכולים להתחבר כרגע" הודעה</span><span class="sxs-lookup"><span data-stu-id="ba337-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="ba337-103">אם תקבל הודעה זו, נסה את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="ba337-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="ba337-104">בדוק את חומת האש, תוכנת האנטי-וירוס והגדרות ה-proxy כדי לוודא שהן אינן חוסמות גישה לאינטרנט ליישומי Office.</span><span class="sxs-lookup"><span data-stu-id="ba337-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="ba337-105">ראה [כתובות Url של Office 365 וטווחי כתובות IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="ba337-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="ba337-106">עבור **להתחלת** > **הפעלה**ולאחר מכן הקלד **services. msc**.</span><span class="sxs-lookup"><span data-stu-id="ba337-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="ba337-107">ודא שהשירותים הבאים פועלים:</span><span class="sxs-lookup"><span data-stu-id="ba337-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="ba337-108">התקנה אוטומטית של התקני רשת מחוברים</span><span class="sxs-lookup"><span data-stu-id="ba337-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="ba337-109">שירות רשימת הרשתות</span><span class="sxs-lookup"><span data-stu-id="ba337-109">Network List Service</span></span>
    - <span data-ttu-id="ba337-110">מיקום רשת מודעות</span><span class="sxs-lookup"><span data-stu-id="ba337-110">Network Location Awareness</span></span>
    - <span data-ttu-id="ba337-111">יומן האירועים של Windows</span><span class="sxs-lookup"><span data-stu-id="ba337-111">Windows Event Log</span></span>

<span data-ttu-id="ba337-112">אם אחד מהשירותים הללו אינו פועל, נסה להפעיל אותו.</span><span class="sxs-lookup"><span data-stu-id="ba337-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="ba337-113">אם יש לך בעיה בהפעלת השירות, הפעל את הפקודה הבאה על-ידי פתיחת שורת פקודה עם הרשאות מוגברות:</span><span class="sxs-lookup"><span data-stu-id="ba337-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="ba337-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="ba337-114">**sfc /scannow**</span></span>

<span data-ttu-id="ba337-115">לאחר סיום פקודה זו, הפעל מחדש את המחשב.</span><span class="sxs-lookup"><span data-stu-id="ba337-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="ba337-116">למידע מפורט, ראה [מצטערים, איננו יכולים להתחבר לחשבונך. נא נסה שוב מאוחר יותר את השגיאה בעת הפעלת Office מ-Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="ba337-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>