---
title: Exchange PowerShell והוצאה משימוש של אימות בסיסי
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
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813473"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="a4183-102">Exchange PowerShell והוצאה משימוש של אימות בסיסי</span><span class="sxs-lookup"><span data-stu-id="a4183-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="a4183-103">לקבלת המידע העדכני ביותר על כיצד להתחבר ל- Exchange Online PowerShell ללא שימוש באימות בסיסי, [עבור לכאן](https://aka.ms/exops-docs).</span><span class="sxs-lookup"><span data-stu-id="a4183-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="a4183-104">מודול PowerShell V2 אינו משתמש באימות בסיסי.</span><span class="sxs-lookup"><span data-stu-id="a4183-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="a4183-105">שים לב שאימות בסיסי עדיין צריך להיות זמין במחשב הלקוח.</span><span class="sxs-lookup"><span data-stu-id="a4183-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="a4183-106">המודול החדש של PowerShell V2 משתמש באימות מודרני כדי ליצור חיבור להפעלה של כל רכיבי V2 Cmdlet מבוססי REST.</span><span class="sxs-lookup"><span data-stu-id="a4183-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="a4183-107">בנוסף לרכיבי V2 cmdlet, הוא גם מאפשר לך לגשת לרכיבים קודמים של Cmdlet של PowerShell מרוחק (RPS), שדורשים הפעלה של PowerShell מרוחק.</span><span class="sxs-lookup"><span data-stu-id="a4183-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="a4183-108">יצירת הפעלת RPS במחשב Windows דורשת ש-WinRM BasicAuth יהיה זמין במחשב הלקוח למרות שהמודול משתמש במנגנון אימות מודרני כדי לאמת את השירות.</span><span class="sxs-lookup"><span data-stu-id="a4183-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="a4183-109">צינור האימות הבסיסי של WinRM משמש להובלת אסימוני אימות מודרניים.</span><span class="sxs-lookup"><span data-stu-id="a4183-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="a4183-110">אם האימות הבסיסי של WinRM אינו זמין במחשב הלקוח, רכיבי ה-V2 cmdlet החדשים ימשיכו לפעול (אך רכיבי ה- cmdlet הקודמים של RPS לא ימשיכו לפעול).</span><span class="sxs-lookup"><span data-stu-id="a4183-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
