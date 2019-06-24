---
title: תקן את השגיאה 0x8004de40 ב- OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133978"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="8b4c8-102">תקן את השגיאה 0x8004de40 ב- OneDrive</span><span class="sxs-lookup"><span data-stu-id="8b4c8-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="8b4c8-103">אם מתקבלת שגיאה 0x8004de40 עם OneDrive:</span><span class="sxs-lookup"><span data-stu-id="8b4c8-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="8b4c8-104">אתחל מחדש את המחשב המושפע במצב מחובר לתחום הספריה Acitve שלך.</span><span class="sxs-lookup"><span data-stu-id="8b4c8-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="8b4c8-105">אם אתחול מחדש לא פותר את הבעיה, הצטרפות לקבוצת והצטרף המכשיר הפרסומת תכלת הרקיע.</span><span class="sxs-lookup"><span data-stu-id="8b4c8-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="8b4c8-106">**הערה**: עליך לנהוג ברשת של החברה שלך בעת ביצוע שלבים אלה.</span><span class="sxs-lookup"><span data-stu-id="8b4c8-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="8b4c8-107">אל תבצע את הפעולות הבאות כאשר אינם יכולים להתחבר תשתית החברה שלך (לדוגמה, בעת נסיעה).</span><span class="sxs-lookup"><span data-stu-id="8b4c8-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="8b4c8-108">פתח שורת פקודה בעלת הרשאות מלאות.</span><span class="sxs-lookup"><span data-stu-id="8b4c8-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="8b4c8-109">כדי לפתוח שורת פקודה בעלת הרשאות מלאות, לחץ על - **התחלה**, לחץ לחיצה ימנית על **שורת הפקודה**ולאחר מכן לחץ על **הפעל כמנהל**.</span><span class="sxs-lookup"><span data-stu-id="8b4c8-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="8b4c8-110">הקלד *dsregcmd /leave* והקש **Enter**.</span><span class="sxs-lookup"><span data-stu-id="8b4c8-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="8b4c8-111">בסיום, הקלד *dsregcmd /join* והקש **Enter**.</span><span class="sxs-lookup"><span data-stu-id="8b4c8-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="8b4c8-112">בסיום, לסגור את שורת הפקודה.</span><span class="sxs-lookup"><span data-stu-id="8b4c8-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="8b4c8-113">אתחל מחדש את המחשב ולאחר מכן היכנס לתוך OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8b4c8-113">Reboot the computer, and log into OneDrive.</span></span>