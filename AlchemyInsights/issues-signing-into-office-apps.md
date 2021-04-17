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
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833004"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="2f10f-102">תיקון אפליקציות Microsoft 365 "מודול הפלטפורמה המהימנה של המחשב שלך אינו פועל כראוי"</span><span class="sxs-lookup"><span data-stu-id="2f10f-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="2f10f-103">כדי לתקן שגיאה זו, נסה את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="2f10f-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="2f10f-104">התקן את העדכונים האחרונים עבור [Windows ו-](https://support.microsoft.com/help/4027667/windows-10-update) [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="2f10f-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="2f10f-105">[נקה אישורי Office](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) באמצעות מנהל האישורים של Windows.</span><span class="sxs-lookup"><span data-stu-id="2f10f-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="2f10f-106">**הערה:** נתיבי הרישום עבור Office 2016 השתנו ל- 16.0.</span><span class="sxs-lookup"><span data-stu-id="2f10f-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="2f10f-107">(לדוגמה: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="2f10f-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="2f10f-108">נסה את [תהליך שחזור המשתמשים כדי](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) לתקן כשלים במודול פלטפורמה מהימנה (TPM).</span><span class="sxs-lookup"><span data-stu-id="2f10f-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="2f10f-109">הגדר את EnableADAL = 0 באמצעות השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="2f10f-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="2f10f-110">לחץ באמצעות לחצן העכבר הימני על לחצן התחל של Windows, **בחר הפעל**, **הקלד regedit** ולאחר מכן בחר **אישור.**</span><span class="sxs-lookup"><span data-stu-id="2f10f-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="2f10f-111">בחר **כן** כדי לאפשר לעורך הרישום לבצע שינויים במכשיר שלך.</span><span class="sxs-lookup"><span data-stu-id="2f10f-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="2f10f-112">בעורך הרישום, הוסף ערך DWORD של **EnableADAL** עם הגדרה של **0 תחת** HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="2f10f-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="2f10f-113">לקבלת מידע נוסף, ראה בעיות חיבור בהתחברות לאחר עדכון ל- [Office 2016 גירסת Build מס' 16.0.7967 ב- Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="2f10f-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>