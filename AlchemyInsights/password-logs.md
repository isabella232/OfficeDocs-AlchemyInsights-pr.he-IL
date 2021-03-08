---
title: יומני סיסמאות
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50525139"
---
# <a name="password-logs"></a><span data-ttu-id="466cb-102">יומני סיסמאות</span><span class="sxs-lookup"><span data-stu-id="466cb-102">Password logs</span></span>

<span data-ttu-id="466cb-103">**אני נתקל בבעיות בגישה ליומני ביקורת של איפוס סיסמאות**</span><span class="sxs-lookup"><span data-stu-id="466cb-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="466cb-104">כדי לפתור בעיות בנוגע לגישה ליומני ביקורת של איפוס סיסמאות, בצע את השלב הבא:</span><span class="sxs-lookup"><span data-stu-id="466cb-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="466cb-105">ודא שאתה מורשה להציג יומני ביקורת.</span><span class="sxs-lookup"><span data-stu-id="466cb-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="466cb-106">רק התפקידים הבאים מורשים:</span><span class="sxs-lookup"><span data-stu-id="466cb-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="466cb-107">מנהל מערכת כללי</span><span class="sxs-lookup"><span data-stu-id="466cb-107">Global administrator</span></span>
 - <span data-ttu-id="466cb-108">מנהל מערכת של אבטחה</span><span class="sxs-lookup"><span data-stu-id="466cb-108">Security administrator</span></span>
 - <span data-ttu-id="466cb-109">קורא האבטחה</span><span class="sxs-lookup"><span data-stu-id="466cb-109">Security reader</span></span>

<span data-ttu-id="466cb-110">**אני מעוניין לראות את כל אירועי הביקורת של איפוס הסיסמאות מהזמן שאני מפרוס לראשונה**</span><span class="sxs-lookup"><span data-stu-id="466cb-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="466cb-111">מתבצעת העברה של עד 120,000 סיסמאות לאיפוס הסיסמה/הרישום מאוחסנים בדוחות של 30 הימים האחרונים.</span><span class="sxs-lookup"><span data-stu-id="466cb-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="466cb-112">מגבלה מרבית זו חלה על ממשק המשתמש בעת הורדת ה-CSV.</span><span class="sxs-lookup"><span data-stu-id="466cb-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="466cb-113">אירועי 1,000,000 זמינים דרך PowerShell.</span><span class="sxs-lookup"><span data-stu-id="466cb-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="466cb-114">לקבלת מידע נוסף, עיין בקישורים הבאים:</span><span class="sxs-lookup"><span data-stu-id="466cb-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="466cb-115">אירועי איפוס סיסמה בשירות עצמי מתוך API של דוחות ואירועים של ' תכלת ואירועים '</span><span class="sxs-lookup"><span data-stu-id="466cb-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="466cb-116">כיצד להוריד את אירועי הרישום לאיפוס סיסמה במהירות באמצעות PowerShell</span><span class="sxs-lookup"><span data-stu-id="466cb-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="466cb-117">**אני מעוניין להבין עוד אודות יכולות דיווח של איפוס סיסמאות**</span><span class="sxs-lookup"><span data-stu-id="466cb-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="466cb-118">בדוק מי נרשם או מאפס סיסמאות באמצעות האפשרות ' איפוס סיסמה של הודעות מיידיות ' בפורטל ' תכלת ' תחת ' **משתמשים וקבוצות**'.</span><span class="sxs-lookup"><span data-stu-id="466cb-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="466cb-119">לקבלת מידע נוסף, עיין בקישורים הבאים:</span><span class="sxs-lookup"><span data-stu-id="466cb-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="466cb-120">מבט כולל על דוחות איפוס סיסמה</span><span class="sxs-lookup"><span data-stu-id="466cb-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="466cb-121">כיצד להציג דוחות של איפוס סיסמאות בפורטל התכלת</span><span class="sxs-lookup"><span data-stu-id="466cb-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="466cb-122">אירועי איפוס סיסמה בשירות עצמי מתוך API של דוחות ואירועים של ' תכלת ואירועים '</span><span class="sxs-lookup"><span data-stu-id="466cb-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="466cb-123">כיצד להוריד את אירועי הרישום לאיפוס סיסמה במהירות באמצעות PowerShell</span><span class="sxs-lookup"><span data-stu-id="466cb-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


