---
title: פתרון בעיות של קריסות ב- OneDrive
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
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826200"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="63736-102">פתרון בעיות של קריסות ב- OneDrive</span><span class="sxs-lookup"><span data-stu-id="63736-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="63736-103">אם OneDrive קורס שוב ושוב, נסה את השלבים הבאים לפתרון בעיות:</span><span class="sxs-lookup"><span data-stu-id="63736-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="63736-104">**ודא שמפתחות הרישום אינם מוגדרים:**</span><span class="sxs-lookup"><span data-stu-id="63736-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="63736-105">באמצעות עורך הרישום, נווט אל HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="63736-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="63736-106">אם DisableFileSyncNGSC קיים ומוגדר ל- 1, פתח את המפתח ושנה את הערך ל- 0.</span><span class="sxs-lookup"><span data-stu-id="63736-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="63736-107">הפעל את OneDrive באופן ידני על-ידי מעבר אל התחל</span><span class="sxs-lookup"><span data-stu-id="63736-107">Manually launch OneDrive by going to Start</span></span> ![הקש על מקש Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="63736-109">, הקלד OneDrive בתיבת החיפוש ולאחר מכן לחץ על אפליקציית שולחן העבודה של OneDrive.</span><span class="sxs-lookup"><span data-stu-id="63736-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="63736-110">**איפוס OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="63736-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="63736-111">הערות:</span><span class="sxs-lookup"><span data-stu-id="63736-111">Notes:</span></span>

- <span data-ttu-id="63736-112">איפוס OneDrive מנתק את כל חיבורי הסינכרון הקיימים שלך (כולל OneDrive האישי שלך אם הוגדר).</span><span class="sxs-lookup"><span data-stu-id="63736-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="63736-113">לא תאבד קבצים או נתונים על-ידי איפוס OneDrive במחשב שלך.</span><span class="sxs-lookup"><span data-stu-id="63736-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="63736-114">**כדי לאפס את OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="63736-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="63736-115">פתח תיבת דו-שיח הפעלה על-ידי הקשה על מקש Windows ו- R.</span><span class="sxs-lookup"><span data-stu-id="63736-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="63736-116">הקלד %localappdata%\Microsoft\OneDrive\onedrive.exe /reset והקש OK.</span><span class="sxs-lookup"><span data-stu-id="63736-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="63736-117">חלון פקודה עשוי להופיע לזמן קצר.</span><span class="sxs-lookup"><span data-stu-id="63736-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="63736-118">הפעל את OneDrive באופן ידני על-ידי מעבר אל התחל</span><span class="sxs-lookup"><span data-stu-id="63736-118">Manually launch OneDrive by going to Start</span></span> ![הקש על מקש Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="63736-120">, הקלד OneDrive בתיבת החיפוש ולאחר מכן לחץ על אפליקציית שולחן העבודה של OneDrive.</span><span class="sxs-lookup"><span data-stu-id="63736-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="63736-121">הערות:</span><span class="sxs-lookup"><span data-stu-id="63736-121">Notes:</span></span>

- <span data-ttu-id="63736-122">אם בחרת לסנכרן רק כמה תיקיות לפני האיפוס, יהיה עליך לעשות זאת שוב לאחר השלמת הסינכרון.</span><span class="sxs-lookup"><span data-stu-id="63736-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="63736-123">קרא [בחר אילו תיקיות OneDrive לסנכרן עם המחשב שלך](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)לקבלת מידע   נוסף.</span><span class="sxs-lookup"><span data-stu-id="63736-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="63736-124">יהיה עליך להשלים פעולה זו עבור OneDrive ו- OneDrive for Business האישיים שלך.</span><span class="sxs-lookup"><span data-stu-id="63736-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>