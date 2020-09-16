---
title: תיקון שגיאת 0x8004de40 ב-OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745131"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="b2c10-102">תיקון שגיאת 0x8004de40 ב-OneDrive</span><span class="sxs-lookup"><span data-stu-id="b2c10-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="b2c10-103">אם אתה מקבל שגיאת 0x8004de40 עם OneDrive:</span><span class="sxs-lookup"><span data-stu-id="b2c10-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="b2c10-104">הפעל מחדש את המחשב המושפע בעת חיבור לתחום מדריך הכתובות שלך ב-Acitve.</span><span class="sxs-lookup"><span data-stu-id="b2c10-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="b2c10-105">אם אתחול מחדש אינו פותר את הבעיה, הצטרף למכשיר והצטרף אליו מחדש מתכלת לספירה.</span><span class="sxs-lookup"><span data-stu-id="b2c10-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="b2c10-106">**הערה**: עליך להיות ברשת החברה שלך בעת ביצוע שלבים אלה.</span><span class="sxs-lookup"><span data-stu-id="b2c10-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="b2c10-107">אל תבצע שלבים אלה כאשר אינך מצליח להתחבר לתשתית הארגונית שלך (לדוגמה, בעת נסיעה).</span><span class="sxs-lookup"><span data-stu-id="b2c10-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="b2c10-108">פתח שורת פקודה מוגבהת.</span><span class="sxs-lookup"><span data-stu-id="b2c10-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="b2c10-109">כדי לפתוח שורת פקודה מוגבהת, לחץ על **התחל**, לחץ באמצעות לחצן העכבר הימני על **שורת הפקודה**ולאחר מכן לחץ על **הפעל כמנהל**.</span><span class="sxs-lookup"><span data-stu-id="b2c10-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="b2c10-110">הקלד *dsregcmd/leave* והקש **Enter**.</span><span class="sxs-lookup"><span data-stu-id="b2c10-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="b2c10-111">כאשר תסיים, הקלד *dsregcmd/join* והקש **Enter**.</span><span class="sxs-lookup"><span data-stu-id="b2c10-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="b2c10-112">כאשר תסיים, סגור את שורת הפקודה.</span><span class="sxs-lookup"><span data-stu-id="b2c10-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="b2c10-113">אתחל מחדש את המחשב והיכנס ל-OneDrive.</span><span class="sxs-lookup"><span data-stu-id="b2c10-113">Reboot the computer, and log into OneDrive.</span></span>