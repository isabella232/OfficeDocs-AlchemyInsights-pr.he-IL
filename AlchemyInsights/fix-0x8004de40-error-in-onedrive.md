---
title: תיקון 0x8004de40 ב- OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649749"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="5682c-102">תיקון 0x8004de40 ב- OneDrive</span><span class="sxs-lookup"><span data-stu-id="5682c-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="5682c-103">אם אתה משתמש ב- Windows 7 ומקבל שגיאה זו, עדכן כדי להפוך [את TLS 1.1 ו- TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)לזמינים כפרוטוקולים מאובטחים המהווים ברירת מחדל ב- WinHTTP ב- Windows.</span><span class="sxs-lookup"><span data-stu-id="5682c-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="5682c-104">אם אתה משתמש ב- Windows 10, ואתה מקבל הודעת 0x8004de40 ב- OneDrive:</span><span class="sxs-lookup"><span data-stu-id="5682c-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="5682c-105">אתחל מחדש את המחשב המושפע בעת חיבור לתחום Acitve Directory שלך.</span><span class="sxs-lookup"><span data-stu-id="5682c-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="5682c-106">אם אתחול מחדש אינו מתקן את הבעיה, בטל את ההסתהוות ו להצטרף שוב למכשיר שלך מ- Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5682c-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="5682c-107">**הערה:** עליך להיות ברשת הארגונית שלך בעת ביצוע שלבים אלה.</span><span class="sxs-lookup"><span data-stu-id="5682c-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="5682c-108">אל תבצע שלבים אלה כאשר אינך מחובר לתשתית הארגונית שלך (לדוגמה, במהלך נסיעה).</span><span class="sxs-lookup"><span data-stu-id="5682c-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="5682c-109">פתח שורת פקודה עם הרשאות מלאות על-ידי בחירה **באפשרות** התחל , לחץ באמצעות לחצן העכבר **הימני** על שורת הפקודה ולאחר מכן בחר הפעל **כמנהל מערכת**.</span><span class="sxs-lookup"><span data-stu-id="5682c-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="5682c-110">הקלד *dsregcmd /leave* והקש **Enter**.</span><span class="sxs-lookup"><span data-stu-id="5682c-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="5682c-111">לאחר ההשלמה, *הקלד dsregcmd /join* והקש **Enter**.</span><span class="sxs-lookup"><span data-stu-id="5682c-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="5682c-112">לאחר ההשלמה, סגור את שורת הפקודה.</span><span class="sxs-lookup"><span data-stu-id="5682c-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="5682c-113">אתחל את המחשב והיכנס ל- OneDrive.</span><span class="sxs-lookup"><span data-stu-id="5682c-113">Reboot the computer, and log into OneDrive.</span></span>