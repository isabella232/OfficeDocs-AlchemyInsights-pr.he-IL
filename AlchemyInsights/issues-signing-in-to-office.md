---
title: בעיות בכניסה לאפליקציות של Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579902"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="2e10e-102">מסך כניסה ריק ב-Microsoft 365 אפליקציות</span><span class="sxs-lookup"><span data-stu-id="2e10e-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="2e10e-103">כדי לפתור בעיה זו, נסה את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="2e10e-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="2e10e-104">התקן את העדכונים האחרונים עבור [Windows](https://support.microsoft.com/help/4027667/windows-10-update) ו- [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="2e10e-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="2e10e-105">איפוס אפשרויות internet explorer: עבור אל **כלים**  >  **אפשרויות אינטרנט**  >  איפוס**מתקדם**  >  **של הגדרות internet explorer** (שים לב שתאבד הגדרות מותאמות אישית) ולאחר מכן נסה שוב להיכנס ל-Office.</span><span class="sxs-lookup"><span data-stu-id="2e10e-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="2e10e-106">בטל את משמר היישומים של Windows Defender (WDAG) או כל חומת אש או תוכנית אנטי-וירוס דומה:</span><span class="sxs-lookup"><span data-stu-id="2e10e-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="2e10e-107">בלוח הבקרה, עבור אל **תוכניות**ולאחר מכן בחר **באפשרות הפעל או בטל את התכונות של Windows**.</span><span class="sxs-lookup"><span data-stu-id="2e10e-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="2e10e-108">אם Windows Defender משמר היישומים מופעל, נסה להשבית אותו.</span><span class="sxs-lookup"><span data-stu-id="2e10e-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="2e10e-109">**הערה:** ייתכן שיהיה עליך להפעיל מחדש את המחשב.</span><span class="sxs-lookup"><span data-stu-id="2e10e-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="2e10e-110">ודא שיישום [plug-In](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) של Microsoft. BROKERPLUGIN עמ מ של מיקרוסופט אינו נחסם על-ידי יישומים או חומת אש/תוכנת אנטי-וירוס כלשהם.</span><span class="sxs-lookup"><span data-stu-id="2e10e-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="2e10e-111">[נקה אישורי Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) באמצעות מנהל האישורים של Windows.</span><span class="sxs-lookup"><span data-stu-id="2e10e-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="2e10e-112">**הערה:** נתיבי הרישום עבור Office 2016 השתנו ל-16.0.</span><span class="sxs-lookup"><span data-stu-id="2e10e-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="2e10e-113">(לשעבר: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="2e10e-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="2e10e-114">לקבלת מידע נוסף, ראה [בעיות חיבור בכניסה לאחר עדכון ל-Office 2016 build 16.0.7967 ב-Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="2e10e-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>