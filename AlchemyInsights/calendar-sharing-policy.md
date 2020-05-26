---
title: 618 מדיניות שיתוף לוח שנה
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373000"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="d3dd1-102">שגיאת מדיניות בעת שיתוף לוח שנה</span><span class="sxs-lookup"><span data-stu-id="d3dd1-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="d3dd1-103">בצע אחת מהפעולות הבאות, בהתאם למצבך:</span><span class="sxs-lookup"><span data-stu-id="d3dd1-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="d3dd1-104">התחבר ל-Exchange Online באמצעות מרחוק PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d3dd1-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="d3dd1-105">לקבלת מידע נוסף, ראה [התחברות ל-Exchange Online באמצעות מרחוק PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="d3dd1-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="d3dd1-106">בשרת המקומי, פתח את מעטפת ניהול Exchange.</span><span class="sxs-lookup"><span data-stu-id="d3dd1-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="d3dd1-107">קבע את מדיניות השיתוף שהוקצתה למשתמש.</span><span class="sxs-lookup"><span data-stu-id="d3dd1-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="d3dd1-108">לשם כך, הפעל את הפקודה הבאה וציין את המדיניות המוחזרת:</span><span class="sxs-lookup"><span data-stu-id="d3dd1-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="d3dd1-109">עדכן את מדיניות השיתוף עבור המשתמש.</span><span class="sxs-lookup"><span data-stu-id="d3dd1-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="d3dd1-110">כדי לעשות זאת, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="d3dd1-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="d3dd1-111">פתח את מרכז הניהול של Exchange.</span><span class="sxs-lookup"><span data-stu-id="d3dd1-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="d3dd1-112">לחץ על **ארגון**ולאחר מכן לחץ פעמיים על המדיניות שהוקצתה למשתמש תחת **שיתוף בודד**.</span><span class="sxs-lookup"><span data-stu-id="d3dd1-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="d3dd1-113">זוהי המדיניות שהוחזרה בשלב 2.</span><span class="sxs-lookup"><span data-stu-id="d3dd1-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="d3dd1-114">בדף ' כלל שיתוף ', בחר ברמת שיתוף לוח השנה שברצונך לאפשר תחת **ציון איזה מידע ברצונך לשתף**; לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="d3dd1-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="d3dd1-115">לקבלת מידע נוסף, ראה: ["מדיניות אינה מאפשרת הענקת הרשאות ברמה זו לאחת או יותר מבין הנמענים" כאשר המשתמש מנסה לשתף לוח שנה](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="d3dd1-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
