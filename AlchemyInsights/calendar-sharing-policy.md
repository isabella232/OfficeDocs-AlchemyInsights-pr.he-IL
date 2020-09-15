---
title: מדיניות שיתוף לוח שנה של 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684231"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="1f0aa-102">שגיאת מדיניות בעת שיתוף לוח שנה</span><span class="sxs-lookup"><span data-stu-id="1f0aa-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="1f0aa-103">בצע אחת מהפעולות הבאות, בהתאם למצב שלך:</span><span class="sxs-lookup"><span data-stu-id="1f0aa-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="1f0aa-104">התחבר ל-Exchange Online באמצעות PowerShell מרוחק.</span><span class="sxs-lookup"><span data-stu-id="1f0aa-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="1f0aa-105">לקבלת מידע נוסף, ראה [התחברות ל-Exchange Online באמצעות PowerShell מרוחק](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="1f0aa-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="1f0aa-106">בשרת המקומי, פתח את מעטפת ניהול Exchange.</span><span class="sxs-lookup"><span data-stu-id="1f0aa-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="1f0aa-107">קבע את מדיניות השיתוף שהוקצתה למשתמש.</span><span class="sxs-lookup"><span data-stu-id="1f0aa-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="1f0aa-108">לשם כך, הפעלת הפקודה הבאה ושימו לב למדיניות המוחזרת:</span><span class="sxs-lookup"><span data-stu-id="1f0aa-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="1f0aa-109">עדכן את מדיניות השיתוף עבור המשתמש.</span><span class="sxs-lookup"><span data-stu-id="1f0aa-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="1f0aa-110">לשם כך, בצע את הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="1f0aa-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="1f0aa-111">פתח את מרכז הניהול של Exchange.</span><span class="sxs-lookup"><span data-stu-id="1f0aa-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="1f0aa-112">לחץ על **ארגון**ולאחר מכן לחץ פעמיים על המדיניות שהוקצתה למשתמש תחת **שיתוף בודד**.</span><span class="sxs-lookup"><span data-stu-id="1f0aa-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="1f0aa-113">זוהי המדיניות שהוחזרה בשלב 2.</span><span class="sxs-lookup"><span data-stu-id="1f0aa-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="1f0aa-114">בדף כלל שיתוף, בחר את רמת השיתוף של לוח השנה שברצונך לאפשר תחת **ציין איזה מידע ברצונך לשתף**; לחץ על **שמור**.</span><span class="sxs-lookup"><span data-stu-id="1f0aa-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="1f0aa-115">לקבלת מידע נוסף, ראה: ["מדיניות אינה מאפשרת הענקת הרשאות ברמה זו לשגיאה אחת או יותר של הנמענים" כאשר המשתמש מנסה לשתף לוח שנה](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="1f0aa-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
