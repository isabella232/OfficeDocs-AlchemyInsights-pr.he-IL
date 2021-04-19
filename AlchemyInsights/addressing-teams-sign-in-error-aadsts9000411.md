---
title: שגיאת כניסה של Teams ל- AADSTS9000411
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
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821988"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="8f956-102">שגיאת כניסה של Teams ל- AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="8f956-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="8f956-103">בעת הכניסה ל- Microsoft Teams, ייתכן שתקבל את השגיאה: מצטערים, אך אנו נתקלים בבעיות בהחתמתך **ב- AADSTS9000411: הבקשה אינה מעוצבת כראוי. הפרמטר "login_hint" משוכפל.**</span><span class="sxs-lookup"><span data-stu-id="8f956-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="8f956-104">כדי לטפל בבעיה זו, ודא שהלקוחות שלך ב- Microsoft Teams מעודכנים.</span><span class="sxs-lookup"><span data-stu-id="8f956-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="8f956-105">לקבלת מידע נוסף אודות עדכון הלקוח שלך, ראה עדכון [Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="8f956-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="8f956-106">אם אין באפשרותך לעדכן את הלקוח מסיבה כלשהי, ביטול הלקוח ינקה את רוב הנתונים המאוחסנים במטמון.</span><span class="sxs-lookup"><span data-stu-id="8f956-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="8f956-107">עם זאת, אם עדיין יש לך בעיות לאחר יציאה/כניסה, צא מ- Teams ונקה את מטמון הלקוח שלך על-ידי ביצוע הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="8f956-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="8f956-108">סגור את Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="8f956-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="8f956-109">עבור אל: %appdata%\microsoft\teams ומחק את כל הקבצים.</span><span class="sxs-lookup"><span data-stu-id="8f956-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="8f956-110">פתח מחדש את Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="8f956-110">Reopen Microsoft Teams.</span></span>
