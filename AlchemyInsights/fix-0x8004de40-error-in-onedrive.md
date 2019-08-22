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
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525060"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="cde70-102">תקן את השגיאה 0x8004de40 ב- OneDrive</span><span class="sxs-lookup"><span data-stu-id="cde70-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="cde70-103">אם מתקבלת שגיאה 0x8004de40 עם OneDrive:</span><span class="sxs-lookup"><span data-stu-id="cde70-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="cde70-104">אתחל מחדש את המחשב המושפע במצב מחובר לתחום הספריה Acitve שלך.</span><span class="sxs-lookup"><span data-stu-id="cde70-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="cde70-105">אם אתחול מחדש לא פותר את הבעיה, הצטרפות לקבוצת והצטרף המכשיר הפרסומת תכלת הרקיע.</span><span class="sxs-lookup"><span data-stu-id="cde70-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="cde70-106">**הערה**: עליך לנהוג ברשת של החברה שלך בעת ביצוע שלבים אלה.</span><span class="sxs-lookup"><span data-stu-id="cde70-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="cde70-107">אל תבצע את הפעולות הבאות כאשר אינם יכולים להתחבר תשתית החברה שלך (לדוגמה, בעת נסיעה).</span><span class="sxs-lookup"><span data-stu-id="cde70-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="cde70-108">פתח שורת פקודה בעלת הרשאות מלאות.</span><span class="sxs-lookup"><span data-stu-id="cde70-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="cde70-109">כדי לפתוח שורת פקודה בעלת הרשאות מלאות, לחץ על - **התחלה**, לחץ לחיצה ימנית על **שורת הפקודה**ולאחר מכן לחץ על **הפעל כמנהל**.</span><span class="sxs-lookup"><span data-stu-id="cde70-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="cde70-110">הקלד *dsregcmd /leave* והקש **Enter**.</span><span class="sxs-lookup"><span data-stu-id="cde70-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="cde70-111">בסיום, הקלד *dsregcmd /join* והקש **Enter**.</span><span class="sxs-lookup"><span data-stu-id="cde70-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="cde70-112">בסיום, לסגור את שורת הפקודה.</span><span class="sxs-lookup"><span data-stu-id="cde70-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="cde70-113">אתחל מחדש את המחשב ולאחר מכן היכנס לתוך OneDrive.</span><span class="sxs-lookup"><span data-stu-id="cde70-113">Reboot the computer, and log into OneDrive.</span></span>