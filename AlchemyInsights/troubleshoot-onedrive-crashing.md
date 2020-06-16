---
title: פתרון בעיות בקריסות של כוננים one
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/15/2020
ms.locfileid: "44748920"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="06b0b-102">פתרון בעיות בקריסות של כוננים one</span><span class="sxs-lookup"><span data-stu-id="06b0b-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="06b0b-103">אם OneDrive מתנגש שוב ושוב, נסה את שלבי פתרון התקלות הבאים:</span><span class="sxs-lookup"><span data-stu-id="06b0b-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="06b0b-104">**ודא שמפתחות הרישום אינם מוגדרים:**</span><span class="sxs-lookup"><span data-stu-id="06b0b-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="06b0b-105">באמצעות עורך הרישום, נווט אל HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="06b0b-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="06b0b-106">אם האפשרות Disאייקובלקובץ Syncngsc מוגדרת ל-1, פתח את המפתח ושנה את הערך ל-0.</span><span class="sxs-lookup"><span data-stu-id="06b0b-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="06b0b-107">הפעלה ידנית של OneDrive על ידי הולך להתחיל</span><span class="sxs-lookup"><span data-stu-id="06b0b-107">Manually launch OneDrive by going to Start</span></span> ![לחץ על מקש Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="06b0b-109">, סוג OneDrive בתיבת החיפוש ולאחר מכן לחץ על יישום OneDrive שולחן העבודה.</span><span class="sxs-lookup"><span data-stu-id="06b0b-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="06b0b-110">**אפס כונן OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="06b0b-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="06b0b-111">ערות</span><span class="sxs-lookup"><span data-stu-id="06b0b-111">Notes:</span></span>

- <span data-ttu-id="06b0b-112">איפוס OneDrive מנתק את כל חיבורי הסינכרון הקיימים (כולל הכונן האישי שלך, אם תגדיר).</span><span class="sxs-lookup"><span data-stu-id="06b0b-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="06b0b-113">לא תאבד קבצים או נתונים על-ידי איפוס כונן OneDrive במחשב שלך.</span><span class="sxs-lookup"><span data-stu-id="06b0b-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="06b0b-114">**כדי לאפס את כונן OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="06b0b-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="06b0b-115">פתח תיבת דו-שיח של הפעלה על-ידי הקשה על מקש Windows ו-R.</span><span class="sxs-lookup"><span data-stu-id="06b0b-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="06b0b-116">הקלד% localappdata% \Microsoft\OneDrive\onedrive.exe /איפוס ולחץ על אישור.</span><span class="sxs-lookup"><span data-stu-id="06b0b-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="06b0b-117">חלון פקודה עשוי להופיע בקצרה.</span><span class="sxs-lookup"><span data-stu-id="06b0b-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="06b0b-118">הפעלה ידנית של OneDrive על ידי הולך להתחיל</span><span class="sxs-lookup"><span data-stu-id="06b0b-118">Manually launch OneDrive by going to Start</span></span> ![לחץ על מקש Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="06b0b-120">, סוג OneDrive בתיבת החיפוש ולאחר מכן לחץ על יישום OneDrive שולחן העבודה.</span><span class="sxs-lookup"><span data-stu-id="06b0b-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="06b0b-121">ערות</span><span class="sxs-lookup"><span data-stu-id="06b0b-121">Notes:</span></span>

- <span data-ttu-id="06b0b-122">אם בחרת לסנכרן תיקיות מסוימות בלבד לפני האיפוס, יהיה עליך לעשות זאת שוב לאחר השלמת הסינכרון.</span><span class="sxs-lookup"><span data-stu-id="06b0b-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="06b0b-123">קרא [בחר באילו תיקיות OneDrive יש לסנכרן למחשב שלך](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   לקבלת מידע נוסף.</span><span class="sxs-lookup"><span data-stu-id="06b0b-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="06b0b-124">יהיה עליך להשלים את זה עבור הכונן האישי שלך OneDrive עבור עסקים.</span><span class="sxs-lookup"><span data-stu-id="06b0b-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>