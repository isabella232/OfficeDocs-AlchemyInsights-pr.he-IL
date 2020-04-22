---
title: תיקון יישומי Office מצטערים, יש לנו הודעה על בעיות שרת זמניות
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764118"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="17c49-102">תיקון יישומי Office "מצטערים, יש לנו בעיות שרת זמניות" הודעה</span><span class="sxs-lookup"><span data-stu-id="17c49-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="17c49-103">אם תקבל הודעה זו, נסה את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="17c49-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="17c49-104">בדוק את חומת האש, תוכנת האנטי-וירוס והגדרות ה-proxy כדי לוודא שהן אינן חוסמות גישה לאינטרנט ליישומי Office.</span><span class="sxs-lookup"><span data-stu-id="17c49-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="17c49-105">ראה [כתובות url וטווחי כתובות IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="17c49-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="17c49-106">עבור **להתחלת** > **הפעלה**ולאחר מכן הקלד **services. msc**.</span><span class="sxs-lookup"><span data-stu-id="17c49-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="17c49-107">ודא שהשירותים הבאים פועלים:</span><span class="sxs-lookup"><span data-stu-id="17c49-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="17c49-108">התקנה אוטומטית של התקני רשת מחוברים</span><span class="sxs-lookup"><span data-stu-id="17c49-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="17c49-109">שירות רשימת הרשתות</span><span class="sxs-lookup"><span data-stu-id="17c49-109">Network List Service</span></span>
    - <span data-ttu-id="17c49-110">מיקום רשת מודעות</span><span class="sxs-lookup"><span data-stu-id="17c49-110">Network Location Awareness</span></span>
    - <span data-ttu-id="17c49-111">יומן האירועים של Windows</span><span class="sxs-lookup"><span data-stu-id="17c49-111">Windows Event Log</span></span>

<span data-ttu-id="17c49-112">אם אחד מהשירותים הללו אינו פועל, נסה להפעיל אותו.</span><span class="sxs-lookup"><span data-stu-id="17c49-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="17c49-113">אם יש לך בעיה בהפעלת השירות, הפעל את הפקודה הבאה על-ידי פתיחת שורת פקודה עם הרשאות מוגברות:</span><span class="sxs-lookup"><span data-stu-id="17c49-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="17c49-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="17c49-114">**sfc /scannow**</span></span>

<span data-ttu-id="17c49-115">לאחר סיום פקודה זו, הפעל מחדש את המחשב.</span><span class="sxs-lookup"><span data-stu-id="17c49-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="17c49-116">למידע מפורט, ראה [מצטערים, איננו יכולים להתחבר לחשבונך. נא נסה שוב מאוחר יותר את השגיאה כאשר אתה מפעיל](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="17c49-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>