---
title: לקוח Teams קורס?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354053"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="27c4e-102">לקוח Teams קורס?</span><span class="sxs-lookup"><span data-stu-id="27c4e-102">Teams client crashing?</span></span>

<span data-ttu-id="27c4e-103">אם לקוח Teams שלך קורס, נסה את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="27c4e-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="27c4e-104">אם אתה משתמש ביישום שולחן העבודה של Teams, [ודא שהיישום מעודכן במלואו](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="27c4e-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="27c4e-105">ודא שכל [כתובות ה-url וטווחי הכתובות של Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) נגישים.</span><span class="sxs-lookup"><span data-stu-id="27c4e-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="27c4e-106">התחבר עם חשבון מנהל הדיירים שלך ובדוק את [לוח הבקרה של שירות בריאות](https://docs.microsoft.com/office365/enterprise/view-service-health) כדי לוודא כי אין הפסקת או השפלה שירות קיים.</span><span class="sxs-lookup"><span data-stu-id="27c4e-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="27c4e-107">הסרת התקנה והתקנה מחדש של יישום הצוותים (קישור)</span><span class="sxs-lookup"><span data-stu-id="27c4e-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="27c4e-108">דפדף אל התיקיה%Appdata%\ute\cos\n במחשב שלך ומחק את כל הקבצים בספריה זו.</span><span class="sxs-lookup"><span data-stu-id="27c4e-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="27c4e-109">[הורד והתקן את יישום הצוותים](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), ואם אפשר, התקן צוותים כמנהל (לחץ לחיצה ימנית על תוכנית ההתקנה של הצוותים ובחר באפשרות "הפעל כמנהל" אם הוא זמין).</span><span class="sxs-lookup"><span data-stu-id="27c4e-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="27c4e-110">אם לקוח הצוותים שלך עדיין מתרסק, האם תוכל לשחזר את הבעיה?</span><span class="sxs-lookup"><span data-stu-id="27c4e-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="27c4e-111">אם כן:</span><span class="sxs-lookup"><span data-stu-id="27c4e-111">If so:</span></span>

1. <span data-ttu-id="27c4e-112">השתמש במקליט השלבים כדי ללכוד את הצעדים שלך.</span><span class="sxs-lookup"><span data-stu-id="27c4e-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="27c4e-113">סגור את כל היישומים המיותרים או הסודיים.</span><span class="sxs-lookup"><span data-stu-id="27c4e-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="27c4e-114">הפעל את מקליט השלבים ושנה את הבעיה בזמן שהתחברת עם חשבון המשתמש המושפע.</span><span class="sxs-lookup"><span data-stu-id="27c4e-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="27c4e-115">[לאסוף את יומני הצוותים כי ללכוד את הצעדים המוקלט כי](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="27c4e-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="27c4e-116">**הערה**: ודא שלכדת את כתובת הכניסה של המשתמש המושפעים.</span><span class="sxs-lookup"><span data-stu-id="27c4e-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="27c4e-117">לאסוף את הקובץ dump ו/או מידע דלי תקלות (Windows).</span><span class="sxs-lookup"><span data-stu-id="27c4e-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="27c4e-118">הפעל את Windows Powershell במחשב שבו ההתרסקות מתרחשת ולהפעיל את הפקודות הבאות:</span><span class="sxs-lookup"><span data-stu-id="27c4e-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="27c4e-119">צרף את הקובץ לתיק התמיכה שלך.</span><span class="sxs-lookup"><span data-stu-id="27c4e-119">Attach the file to your support case.</span></span>
