---
title: Teams לקוח קורס
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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187722"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="05a3a-102">Teams לקוח קורס</span><span class="sxs-lookup"><span data-stu-id="05a3a-102">Teams client crashing</span></span>

<span data-ttu-id="05a3a-103">אם לקוח Teams שלך קורס, נסה את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="05a3a-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="05a3a-104">אם אתה משתמש ביישום שולחן העבודה של Teams, [ודא שהיישום מעודכן במלואו](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="05a3a-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="05a3a-105">ודא שכל כתובות [Microsoft 365 הכתובות וטווחי הכתובות](/microsoftteams/connectivity-issues) נגישים.</span><span class="sxs-lookup"><span data-stu-id="05a3a-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="05a3a-106">היכנס באמצעות חשבון מנהל הדייר שלך ובדוק את לוח [המחוונים](/office365/enterprise/view-service-health) של תקינות השירות כדי לוודא שלא קיימים בעיות של מחסור או שפלת שירות.</span><span class="sxs-lookup"><span data-stu-id="05a3a-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="05a3a-107">הסרת התקנה והתקנה מחדש של Teams היישום</span><span class="sxs-lookup"><span data-stu-id="05a3a-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="05a3a-108">עבור אל התיקיה %appdata%\Microsoft\Teams\ במחשב שלך ומחק את כל הקבצים במדריך כתובות זה.</span><span class="sxs-lookup"><span data-stu-id="05a3a-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="05a3a-109">[הורד והתקן את יישום Teams](https://www.microsoft.com/microsoft-teams/download-app), ואם הדבר אפשרי, התקן Teams כמנהל מערכת (לחץ באמצעות לחצן העכבר הימני על Teams תוכנית ההתקנה ובחר **הפעל** כמנהל מערכת אם זמין).</span><span class="sxs-lookup"><span data-stu-id="05a3a-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="05a3a-110">אם Teams שלך עדיין קורס, נסה לשחזר את הבעיה.</span><span class="sxs-lookup"><span data-stu-id="05a3a-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="05a3a-111">אם תוכל:</span><span class="sxs-lookup"><span data-stu-id="05a3a-111">If you can:</span></span>

1. <span data-ttu-id="05a3a-112">השתמש במקליט השלבים כדי ללכוד את השלבים שלך.</span><span class="sxs-lookup"><span data-stu-id="05a3a-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="05a3a-113">סגור את ALL יישומים לא נחוצים או סודיים.</span><span class="sxs-lookup"><span data-stu-id="05a3a-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="05a3a-114">הפעל את מקליט השלבים ושכפול הבעיה בעת כניסה באמצעות חשבון המשתמש המושפע.</span><span class="sxs-lookup"><span data-stu-id="05a3a-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="05a3a-115">[אסוף את יומני הרישום של הצוותים שלכודים את שלבי השכפול המוקלטים.](/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="05a3a-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="05a3a-116">**הערה:** הקפד ללכוד את כתובת הכניסה של המשתמש מושפע.</span><span class="sxs-lookup"><span data-stu-id="05a3a-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="05a3a-117">אסוף את פרטי ה- dump ו/או הדלי של תקלות (Windows).</span><span class="sxs-lookup"><span data-stu-id="05a3a-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="05a3a-118">הפעל Windows Powershell במחשב שבו מתרחשת קריסה ולהפעיל את הפקודות הבאות (לאחר כל פקודה, הקש Enter):</span><span class="sxs-lookup"><span data-stu-id="05a3a-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="05a3a-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="05a3a-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="05a3a-120">לאחר יצירת קובץ הטקסט ומופיע על המסך, שמור את הקובץ וצרף אותו לבקשת השירות.</span><span class="sxs-lookup"><span data-stu-id="05a3a-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
