---
title: לקוח Teams קורס?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826272"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="e3651-102">לקוח Teams קורס?</span><span class="sxs-lookup"><span data-stu-id="e3651-102">Teams client crashing?</span></span>

<span data-ttu-id="e3651-103">אם לקוח Teams שלך קורס, נסה את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="e3651-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="e3651-104">אם אתה משתמש ביישום שולחן העבודה של Teams, [ודא שהיישום מעודכן במלואו](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="e3651-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="e3651-105">ודא שכל כתובות ה- [URL וטווחי הכתובות של Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) נגישות.</span><span class="sxs-lookup"><span data-stu-id="e3651-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="e3651-106">היכנס באמצעות חשבון מנהל הדייר שלך ובדוק את לוח [המחוונים](https://docs.microsoft.com/office365/enterprise/view-service-health) של תקינות השירות כדי לוודא שלא קיימים בעיות של מחסור או שפלת שירות.</span><span class="sxs-lookup"><span data-stu-id="e3651-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="e3651-107">הסרת התקנה והתקנה מחדש של יישום Teams (קישור)</span><span class="sxs-lookup"><span data-stu-id="e3651-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="e3651-108">עבור אל התיקיה %appdata%\Microsoft\teams\ במחשב שלך ומחק את כל הקבצים במדריך כתובות זה.</span><span class="sxs-lookup"><span data-stu-id="e3651-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="e3651-109">[הורד והתקן את היישום Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), ואם הדבר אפשרי, התקן את Teams כמנהל מערכת (לחץ באמצעות לחצן העכבר הימני על המתקין Teams ובחר "הפעל כמנהל" אם זמין).</span><span class="sxs-lookup"><span data-stu-id="e3651-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="e3651-110">אם לקוח Teams שלך עדיין קורס, תוכל לשחזר את הבעיה?</span><span class="sxs-lookup"><span data-stu-id="e3651-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="e3651-111">אם כן:</span><span class="sxs-lookup"><span data-stu-id="e3651-111">If so:</span></span>

1. <span data-ttu-id="e3651-112">השתמש במקליט השלבים כדי ללכוד את השלבים שלך.</span><span class="sxs-lookup"><span data-stu-id="e3651-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="e3651-113">סגור את ALL יישומים לא נחוצים או סודיים.</span><span class="sxs-lookup"><span data-stu-id="e3651-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="e3651-114">הפעל את מקליט השלבים ושכפול הבעיה בעת כניסה באמצעות חשבון המשתמש המושפע.</span><span class="sxs-lookup"><span data-stu-id="e3651-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="e3651-115">[אסוף את יומני הרישום של הצוותים שלכודים את שלבי השכפול המוקלטים.](https://docs.microsoft.com/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="e3651-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="e3651-116">**הערה:** הקפד ללכוד את כתובת הכניסה של המשתמש מושפע.</span><span class="sxs-lookup"><span data-stu-id="e3651-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="e3651-117">אסוף את פרטי ה- dump ו/או הדלי של תקלות (Windows).</span><span class="sxs-lookup"><span data-stu-id="e3651-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="e3651-118">הפעל את Windows Powershell במחשב שבו מתרחשת קריסה ולהפעיל את הפקודות הבאות:</span><span class="sxs-lookup"><span data-stu-id="e3651-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="e3651-119">צרף את הקובץ למקרה התמיכה שלך.</span><span class="sxs-lookup"><span data-stu-id="e3651-119">Attach the file to your support case.</span></span>
