---
title: בעיות הכניסה אל יישומי Office
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
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938231"
---
# <a name="blank-sign-in-screen-in-office-apps"></a><span data-ttu-id="2809c-102">מסך הכניסה ריק ב- Office apps</span><span class="sxs-lookup"><span data-stu-id="2809c-102">Blank sign-in screen in Office apps</span></span>

<span data-ttu-id="2809c-103">כדי לפתור בעיה זו, נסה את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="2809c-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="2809c-104">התקן את העדכונים האחרונים עבור [Windows](https://support.microsoft.com/help/4027667/windows-10-update) ו- [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="2809c-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="2809c-105">איפוס Internet Explorer אפשרויות: עבור אל **כלי** > **אפשרויות אינטרנט** > **מתקדם** > **איפוס הגדרות Internet Explorer** (הערה תאבד את הגדרות מותאמות אישית) ולאחר מכן נסה שוב להיכנס ל- Office.</span><span class="sxs-lookup"><span data-stu-id="2809c-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="2809c-106">השבת את מגן יישום של Windows Defender (WDAG) או כל תוכנית חומת אש או אנטי-וירוס דומה:</span><span class="sxs-lookup"><span data-stu-id="2809c-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="2809c-107">בלוח הבקרה, לעבור על **תוכניות**ולאחר מכן בחר את **תכונות Windows להפעיל או לבטל**.</span><span class="sxs-lookup"><span data-stu-id="2809c-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="2809c-108">אם מגן יישום של Windows Defender זמינה, נסה להפוך אותה ללא זמינה.</span><span class="sxs-lookup"><span data-stu-id="2809c-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="2809c-109">**הערה:** ייתכן שיהיה עליך להפעיל מחדש את המחשב.</span><span class="sxs-lookup"><span data-stu-id="2809c-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="2809c-110">ודא כי Microsoft.AAD.BrokerPlugin [WAM AAD יישום plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) אינה חסומה על-ידי כל יישום או תוכנית חומת אש/anti-virus.</span><span class="sxs-lookup"><span data-stu-id="2809c-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="2809c-111">[אישורי Office ניקוי](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) באמצעות מנהל האישורים של Windows.</span><span class="sxs-lookup"><span data-stu-id="2809c-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="2809c-112">**הערה:** נתיבי רישום עבור Office 2016 השתנו כדי 16.0.</span><span class="sxs-lookup"><span data-stu-id="2809c-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="2809c-113">(לדוגמה: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="2809c-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="2809c-114">לקבלת מידע נוסף, ראה [חיבור בעיות בהכניסה לאחר העדכון ל- Office 2016 build 16.0.7967 על Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="2809c-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>