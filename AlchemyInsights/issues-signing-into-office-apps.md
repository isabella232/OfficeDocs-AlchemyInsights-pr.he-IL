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
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938232"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="2a9d6-102">תיקון ההודעה "מודול פלטפורמה מהימנים של המחשב שלך אינו פועל כראוי" יישומי Office</span><span class="sxs-lookup"><span data-stu-id="2a9d6-102">Fixing the Office apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="2a9d6-103">כדי לתקן שגיאה זו, נסה לבצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="2a9d6-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="2a9d6-104">התקן את העדכונים האחרונים עבור [Windows](https://support.microsoft.com/help/4027667/windows-10-update) ו- [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="2a9d6-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="2a9d6-105">[אישורי Office ניקוי](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) באמצעות מנהל האישורים של Windows.</span><span class="sxs-lookup"><span data-stu-id="2a9d6-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="2a9d6-106">**הערה:** נתיבי רישום עבור Office 2016 השתנו כדי 16.0.</span><span class="sxs-lookup"><span data-stu-id="2a9d6-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="2a9d6-107">(לדוגמה: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="2a9d6-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="2a9d6-108">נסה את [תהליך השחזור של המשתמש](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) כדי לתקן כשלים Trusted Platform Module (TPM).</span><span class="sxs-lookup"><span data-stu-id="2a9d6-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="2a9d6-109">הגדר את EnableADAL = 0 באמצעות השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="2a9d6-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="2a9d6-110">באמצעות לחצן העכבר הימני על לחצן התחל של Windows, בחר באפשרות **הפעל**, הקלד **regedit**ולאחר מכן לחץ על **אישור**.</span><span class="sxs-lookup"><span data-stu-id="2a9d6-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="2a9d6-111">בחר **כן** כדי לאפשר בעורך הרישום כדי לבצע שינויים למכשיר שלך.</span><span class="sxs-lookup"><span data-stu-id="2a9d6-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="2a9d6-112">בעורך הרישום, הוסף ערך DWORD של **EnableADAL** עם הגדרה של **0** תחת HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="2a9d6-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="2a9d6-113">לקבלת מידע נוסף, ראה [חיבור בעיות בהכניסה לאחר העדכון ל- Office 2016 build 16.0.7967 על Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="2a9d6-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>