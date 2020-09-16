---
title: בעיית הפעלה-אין באפשרותנו להתחבר כרגע
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
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725984"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="a1a72-102">תיקון יישומי Microsoft 365 "אין באפשרותנו להתחבר כעת"</span><span class="sxs-lookup"><span data-stu-id="a1a72-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="a1a72-103">אם אתה מקבל הודעה זו, נסה את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="a1a72-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="a1a72-104">בדוק את חומת האש, תוכנת האנטי-וירוס והגדרות ה-proxy כדי לוודא שהם אינם חוסמים את הגישה לאינטרנט ליישומי Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a1a72-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="a1a72-105">ראה [כתובות url וטווחי כתובות IP של Microsoft](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="a1a72-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="a1a72-106">עבור אל **התחל**  >  **להפעיל**ולאחר מכן הקלד **services. msc**.</span><span class="sxs-lookup"><span data-stu-id="a1a72-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="a1a72-107">ודא שהשירותים הבאים פועלים כולם:</span><span class="sxs-lookup"><span data-stu-id="a1a72-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="a1a72-108">התקנה אוטומטית של התקנים מחוברים לרשת</span><span class="sxs-lookup"><span data-stu-id="a1a72-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="a1a72-109">שירות רשימת הרשתות</span><span class="sxs-lookup"><span data-stu-id="a1a72-109">Network List Service</span></span>
    - <span data-ttu-id="a1a72-110">מודעות למיקום ברשת</span><span class="sxs-lookup"><span data-stu-id="a1a72-110">Network Location Awareness</span></span>
    - <span data-ttu-id="a1a72-111">יומן האירועים של Windows</span><span class="sxs-lookup"><span data-stu-id="a1a72-111">Windows Event Log</span></span>

<span data-ttu-id="a1a72-112">אם אחד מהשירותים האלה אינו פועל, נסה להפעיל אותו.</span><span class="sxs-lookup"><span data-stu-id="a1a72-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="a1a72-113">אם אתה נתקל בבעיה בהפעלת השירות, הפעלת הפקודה הבאה על-ידי פתיחת שורת פקודה עם הרשאות מלאות:</span><span class="sxs-lookup"><span data-stu-id="a1a72-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="a1a72-114">**sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="a1a72-114">**sfc /scannow**</span></span>

<span data-ttu-id="a1a72-115">לאחר שפקודה זו מסתיימת, הפעל מחדש את המחשב.</span><span class="sxs-lookup"><span data-stu-id="a1a72-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="a1a72-116">לקבלת מידע מפורט, ראה ["מצטערים, אין לנו אפשרות להתחבר לחשבון שלך. נסה שוב מאוחר יותר את השגיאה כאשר אתה מפעיל את Office מ-Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="a1a72-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>