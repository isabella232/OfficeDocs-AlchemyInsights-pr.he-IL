---
title: Exchange PowerShell והוצאה משימוש של אימות בסיסי
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015690"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="880a3-102">Exchange PowerShell והוצאה משימוש של אימות בסיסי</span><span class="sxs-lookup"><span data-stu-id="880a3-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="880a3-103">לקבלת המידע העדכני ביותר על כיצד להתחבר ל- Exchange Online PowerShell ללא שימוש באימות בסיסי, [עבור לכאן](https://aka.ms/psbasicauth).</span><span class="sxs-lookup"><span data-stu-id="880a3-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/psbasicauth).</span></span>

<span data-ttu-id="880a3-104">שים לב שאימות בסיסי עדיין צריך להיות זמין במחשב הלקוח.</span><span class="sxs-lookup"><span data-stu-id="880a3-104">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="880a3-105">המודול החדש של PowerShell V2 משתמש באימות מודרני כדי ליצור חיבור להפעלה של כל רכיבי V2 Cmdlet מבוססי REST.</span><span class="sxs-lookup"><span data-stu-id="880a3-105">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="880a3-106">בנוסף לרכיבי V2 cmdlet, הוא גם מאפשר לך לגשת לרכיבים קודמים של Cmdlet של PowerShell מרוחק (RPS), שדורשים הפעלה של PowerShell מרוחק.</span><span class="sxs-lookup"><span data-stu-id="880a3-106">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="880a3-107">יצירת הפעלת RPS במחשב Windows דורשת ש-WinRM BasicAuth יהיה זמין במחשב הלקוח למרות שהמודול משתמש במנגנון אימות מודרני כדי לאמת את השירות.</span><span class="sxs-lookup"><span data-stu-id="880a3-107">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="880a3-108">צינור האימות הבסיסי של WinRM משמש להובלת אסימוני אימות מודרניים.</span><span class="sxs-lookup"><span data-stu-id="880a3-108">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="880a3-109">אם האימות הבסיסי של WinRM אינו זמין במחשב הלקוח, רכיבי ה-V2 cmdlet החדשים ימשיכו לפעול (אך רכיבי ה- cmdlet הקודמים של RPS לא ימשיכו לפעול).</span><span class="sxs-lookup"><span data-stu-id="880a3-109">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
