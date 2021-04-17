---
title: בעיות בכניסה לאפליקציות Microsoft 365
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
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833040"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="64f78-102">מסך כניסה ריק באפליקציות Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="64f78-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="64f78-103">כדי לפתור בעיה זו, נסה את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="64f78-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="64f78-104">התקן את העדכונים האחרונים עבור [Windows ו-](https://support.microsoft.com/help/4027667/windows-10-update) [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="64f78-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="64f78-105">איפוס אפשרויות Internet Explorer: עבור **אל** כלים אפשרויות אינטרנט הגדרות מתקדמות של איפוס Internet Explorer (שים לב שתאבד  >    >    >   הגדרות מותאמות אישית) ולאחר מכן נסה שוב להיכנס ל- Office.</span><span class="sxs-lookup"><span data-stu-id="64f78-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="64f78-106">הפוך את Windows Defender Application Guard (WDAG) ללא זמין או כל חומת אש דומה או תוכנית אנטי-וירוס:</span><span class="sxs-lookup"><span data-stu-id="64f78-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="64f78-107">בלוח הבקרה, עבור אל **תוכניות** ולאחר מכן בחר **הפעל או בטל תכונות Windows**.</span><span class="sxs-lookup"><span data-stu-id="64f78-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="64f78-108">אם Windows Defender Application Guard זמין, נסה להפוך אותו ללא זמין.</span><span class="sxs-lookup"><span data-stu-id="64f78-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="64f78-109">**הערה:** ייתכן שיהיה עליך להפעיל מחדש את המחשב.</span><span class="sxs-lookup"><span data-stu-id="64f78-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="64f78-110">ודא ש- Plug-in של Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) אינו נחסם על-ידי יישום או חומת אש/תוכנית אנטי-וירוס.</span><span class="sxs-lookup"><span data-stu-id="64f78-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="64f78-111">[נקה אישורי Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) באמצעות מנהל האישורים של Windows.</span><span class="sxs-lookup"><span data-stu-id="64f78-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="64f78-112">**הערה:** נתיבי הרישום עבור Office 2016 השתנו ל- 16.0.</span><span class="sxs-lookup"><span data-stu-id="64f78-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="64f78-113">(לדוגמה: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="64f78-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="64f78-114">לקבלת מידע נוסף, ראה בעיות חיבור בהתחברות לאחר עדכון ל- [Office 2016 גירסת Build מס' 16.0.7967 ב- Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="64f78-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>