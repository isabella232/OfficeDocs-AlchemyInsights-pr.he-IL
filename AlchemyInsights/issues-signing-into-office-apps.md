---
title: בעיות בכניסה ליישומי Microsoft 365
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
- "9000571"
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695180"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="7558b-102">תיקון יישומי Microsoft 365 "מודול הפלטפורמה המהימנה של המחשב שלך אינו פועל כהלכה"</span><span class="sxs-lookup"><span data-stu-id="7558b-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="7558b-103">כדי לתקן שגיאה זו, נסה את השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="7558b-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="7558b-104">התקן את העדכונים האחרונים עבור [Windows](https://support.microsoft.com/help/4027667/windows-10-update) ו- [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="7558b-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="7558b-105">[נקה את אישורי Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) באמצעות מנהל האישורים של Windows.</span><span class="sxs-lookup"><span data-stu-id="7558b-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="7558b-106">**הערה:** נתיבי הרישום של Office 2016 השתנו ל-16.0.</span><span class="sxs-lookup"><span data-stu-id="7558b-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="7558b-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="7558b-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="7558b-108">נסה את [תהליך שחזור המשתמש](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) כדי לתקן כשלים של מודול פלטפורמה מהימנה (TPM).</span><span class="sxs-lookup"><span data-stu-id="7558b-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="7558b-109">הגדר את EnableADAL = 0 באמצעות השלבים הבאים:</span><span class="sxs-lookup"><span data-stu-id="7558b-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="7558b-110">לחץ באמצעות לחצן העכבר הימני על לחצן התחל של Windows, בחר **הפעל**, הקלד **regedit**ולאחר מכן בחר **אישור**.</span><span class="sxs-lookup"><span data-stu-id="7558b-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="7558b-111">בחר **כן** כדי לאפשר לעורך הרישום לבצע שינויים במכשיר שלך.</span><span class="sxs-lookup"><span data-stu-id="7558b-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="7558b-112">בעורך הרישום, הוסף ערך DWORD של **EnableADAL** עם הגדרה של **0** תחת HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.</span><span class="sxs-lookup"><span data-stu-id="7558b-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="7558b-113">לקבלת מידע נוסף, ראה [בעיות חיבור בכניסה לאחר עדכון ל-Office 2016 build 16.0.7967 ב-Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="7558b-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>