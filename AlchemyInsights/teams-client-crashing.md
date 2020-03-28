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
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030582"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="278e5-102">לקוח Teams קורס?</span><span class="sxs-lookup"><span data-stu-id="278e5-102">Teams client crashing?</span></span>

<span data-ttu-id="278e5-103">אם לקוח Teams שלך קורס, נסה את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="278e5-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="278e5-104">אם אתה משתמש ביישום שולחן העבודה של Teams, [ודא שהיישום מעודכן במלואו](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="278e5-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="278e5-105">ודא שכל [כתובת ה-URL של Office 365 וטווחי הכתובות](https://docs.microsoft.com/microsoftteams/connectivity-issues) נגישים.</span><span class="sxs-lookup"><span data-stu-id="278e5-105">Make sure all the [Office 365 URL's and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="278e5-106">היכנס עם חשבון מנהל המערכת שלך ובדוק את [לוח המחוונים של תקינות השירות](https://docs.microsoft.com/office365/enterprise/view-service-health) כדי לאמת שלא קיימות הפסקות חשמל או ירידה בביצועי השירות.</span><span class="sxs-lookup"><span data-stu-id="278e5-106">Log in with your admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="278e5-107">כצעד אחרון, באפשרותך לנסות לנקות את המטמון של לקוח Teams:</span><span class="sxs-lookup"><span data-stu-id="278e5-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="278e5-108">צא לחלוטין מלקוח שולחן העבודה של Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="278e5-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="278e5-109">באפשרותך ללחוץ בעזרת לחצן העכבר הימני על **Teams** מתוך מגש הסמל וללחוץ על **צא**, או להפעיל את מנהל המשימות ולעצור לגמרי את התהליך.</span><span class="sxs-lookup"><span data-stu-id="278e5-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="278e5-110">עבור אל סייר הקבצים והקלד %appdata%\Microsoft\teams.</span><span class="sxs-lookup"><span data-stu-id="278e5-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="278e5-111">לאחר שתיכנס אל מדריך הכתובות, תראה כמה מהתיקיות הבאות:</span><span class="sxs-lookup"><span data-stu-id="278e5-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="278e5-112">מתוך **מטמון יישום**, עבור אל מטמון ומחק את כל הקבצים במיקום המטמון:  %appdata%\Microsoft\teams\application cache\cache.</span><span class="sxs-lookup"><span data-stu-id="278e5-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="278e5-113">מתוך **Blob_storage**, מחק את כל הקבצים: %appdata%\Microsoft\teams\blob_storage.</span><span class="sxs-lookup"><span data-stu-id="278e5-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="278e5-114">מתוך **מטמון**, מחק את כל קבצים: %appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="278e5-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="278e5-115">מתוך **מסדי נתונים**, מחק את כל קבצים: %appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="278e5-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="278e5-116">מתוך **GPUCache**, מחק את כל קבצים: %appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="278e5-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="278e5-117">מתוך **IndexedDB**, מחק את קובץ ה-.db: %appdata%\Microsoft\teams\IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="278e5-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="278e5-118">מתוך **אחסון מקומי**, מחק את כל הקבצים: %appdata%\Microsoft\teams\Local Storage.</span><span class="sxs-lookup"><span data-stu-id="278e5-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="278e5-119">לבסוף, מתוך **tmp**, מחק את כל קבצי: %appdata%\Microsoft\teams\tmp.</span><span class="sxs-lookup"><span data-stu-id="278e5-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="278e5-120">הפעל מחדש את לקוח Teams שלך.</span><span class="sxs-lookup"><span data-stu-id="278e5-120">Restart your Teams client.</span></span>
