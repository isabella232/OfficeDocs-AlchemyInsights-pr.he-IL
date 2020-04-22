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
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716173"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="8f044-102">תיקון האפליקציות של Office "אנחנו לא יכולים להתחבר כרגע" הודעה</span><span class="sxs-lookup"><span data-stu-id="8f044-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="8f044-103">אם תקבל הודעה זו, נסה את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="8f044-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="8f044-104">בדוק את חומת האש, תוכנת האנטי-וירוס והגדרות ה-proxy כדי לוודא שהן אינן חוסמות גישה לאינטרנט ליישומי Office.</span><span class="sxs-lookup"><span data-stu-id="8f044-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="8f044-105">ראה [כתובות url וטווחי כתובות IP של Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="8f044-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="8f044-106">עבור **להתחלת** > **הפעלה**ולאחר מכן הקלד **services. msc**.</span><span class="sxs-lookup"><span data-stu-id="8f044-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="8f044-107">ודא שהשירותים הבאים פועלים:</span><span class="sxs-lookup"><span data-stu-id="8f044-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="8f044-108">התקנה אוטומטית של התקני רשת מחוברים</span><span class="sxs-lookup"><span data-stu-id="8f044-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="8f044-109">שירות רשימת הרשתות</span><span class="sxs-lookup"><span data-stu-id="8f044-109">Network List Service</span></span>
    - <span data-ttu-id="8f044-110">מיקום רשת מודעות</span><span class="sxs-lookup"><span data-stu-id="8f044-110">Network Location Awareness</span></span>
    - <span data-ttu-id="8f044-111">יומן האירועים של Windows</span><span class="sxs-lookup"><span data-stu-id="8f044-111">Windows Event Log</span></span>

<span data-ttu-id="8f044-112">אם אחד מהשירותים הללו אינו פועל, נסה להפעיל אותו.</span><span class="sxs-lookup"><span data-stu-id="8f044-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="8f044-113">אם יש לך בעיה בהפעלת השירות, הפעל את הפקודה הבאה על-ידי פתיחת שורת פקודה עם הרשאות מוגברות:</span><span class="sxs-lookup"><span data-stu-id="8f044-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="8f044-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="8f044-114">**sfc /scannow**</span></span>

<span data-ttu-id="8f044-115">לאחר סיום פקודה זו, הפעל מחדש את המחשב.</span><span class="sxs-lookup"><span data-stu-id="8f044-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="8f044-116">למידע מפורט, ראה [מצטערים, איננו יכולים להתחבר לחשבונך. נא נסה שוב מאוחר יותר את השגיאה בעת הפעלת Office מ-Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="8f044-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>