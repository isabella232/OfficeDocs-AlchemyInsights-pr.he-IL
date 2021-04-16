---
title: בעיית הפעלה - אין באפשרותנו להתחבר כעת
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806443"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="afc31-102">תיקון ההודעה של יישומי Microsoft 365 "אין באפשרותנו להתחבר כעת"</span><span class="sxs-lookup"><span data-stu-id="afc31-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="afc31-103">אם אתה מקבל הודעה זו, נסה את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="afc31-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="afc31-104">בדוק את הגדרות חומת האש, תוכנת האנטי-וירוס וה- Proxy כדי לוודא שהם אינם חוסמים גישה לאינטרנט לאפליקציות Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="afc31-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="afc31-105">ראה [כתובות URL של Microsoft וטווחי כתובות IP.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="afc31-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="afc31-106">עבור אל  >  **התחל הפעלה** ולאחר מכן הקלד **services.msc**.</span><span class="sxs-lookup"><span data-stu-id="afc31-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="afc31-107">ודא שהשירותים הבאים פועלים כולם:</span><span class="sxs-lookup"><span data-stu-id="afc31-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="afc31-108">התקנה אוטומטית של מכשירים מחוברים לרשת</span><span class="sxs-lookup"><span data-stu-id="afc31-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="afc31-109">שירות רשימת רשת</span><span class="sxs-lookup"><span data-stu-id="afc31-109">Network List Service</span></span>
    - <span data-ttu-id="afc31-110">המודעות למיקום ברשת</span><span class="sxs-lookup"><span data-stu-id="afc31-110">Network Location Awareness</span></span>
    - <span data-ttu-id="afc31-111">יומן האירועים של Windows</span><span class="sxs-lookup"><span data-stu-id="afc31-111">Windows Event Log</span></span>

<span data-ttu-id="afc31-112">אם אחד מהשירותים הללו אינו פועל, נסה להפעיל אותו.</span><span class="sxs-lookup"><span data-stu-id="afc31-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="afc31-113">אם יש לך בעיה בה הפעלת השירות, הפעל את הפקודה הבאה על-ידי פתיחת שורת פקודה עם הרשאות מלאות:</span><span class="sxs-lookup"><span data-stu-id="afc31-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="afc31-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="afc31-114">**sfc /scannow**</span></span>

<span data-ttu-id="afc31-115">לאחר סיום פקודה זו, הפעל מחדש את המחשב.</span><span class="sxs-lookup"><span data-stu-id="afc31-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="afc31-116">לקבלת מידע מפורט, [ראה "מצטערים, אין לנו אפשרות להתחבר לחשבון שלך. נסה שוב מאוחר יותר" שגיאה בעת הפעלת Office מ- Microsoft 365.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="afc31-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>