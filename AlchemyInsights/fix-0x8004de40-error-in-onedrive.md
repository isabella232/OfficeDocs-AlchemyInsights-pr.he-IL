---
title: תקן את השגיאה 0x8004de40 ב OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716029"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="fe5f1-102">תקן את השגיאה 0x8004de40 ב OneDrive</span><span class="sxs-lookup"><span data-stu-id="fe5f1-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="fe5f1-103">אם אתה מקבל שגיאת 0x8004de40 עם OneDrive:</span><span class="sxs-lookup"><span data-stu-id="fe5f1-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="fe5f1-104">אתחל מחדש את המחשב המושפע בעת ההתחברות לקבוצת המחשבים של ספריית Acitve.</span><span class="sxs-lookup"><span data-stu-id="fe5f1-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="fe5f1-105">אם אתחול מחדש אינו מתקן את הבעיה, בטל את הצירוף והצטרף מחדש להתקן מתכלת AD.</span><span class="sxs-lookup"><span data-stu-id="fe5f1-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="fe5f1-106">**הערה**: עליך להיות ברשת החברה שלך בעת ביצוע שלבים אלה.</span><span class="sxs-lookup"><span data-stu-id="fe5f1-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="fe5f1-107">אל תבצע שלבים אלה כאשר אינך מצליח להתחבר לתשתית הארגונית (לדוגמה, בעת נסיעה).</span><span class="sxs-lookup"><span data-stu-id="fe5f1-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="fe5f1-108">פתח שורת פקודה עם הרשאות מלאות.</span><span class="sxs-lookup"><span data-stu-id="fe5f1-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="fe5f1-109">כדי לפתוח שורת פקודה מוגבה, לחץ על **התחל**, לחץ לחיצה ימנית על **שורת הפקודה**ולאחר מכן לחץ על **הפעל כמנהל**.</span><span class="sxs-lookup"><span data-stu-id="fe5f1-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="fe5f1-110">הקלד *dsregcmd/השאר* והקש **Enter**.</span><span class="sxs-lookup"><span data-stu-id="fe5f1-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="fe5f1-111">בעת השלמתו, הקלד *dsregcmd/join* והקש **Enter**.</span><span class="sxs-lookup"><span data-stu-id="fe5f1-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="fe5f1-112">לאחר השלמתו, סגור את שורת הפקודה.</span><span class="sxs-lookup"><span data-stu-id="fe5f1-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="fe5f1-113">אתחל את המחשב והיכנס למערכת OneDrive.</span><span class="sxs-lookup"><span data-stu-id="fe5f1-113">Reboot the computer, and log into OneDrive.</span></span>