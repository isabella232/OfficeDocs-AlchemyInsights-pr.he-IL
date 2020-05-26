---
title: שגיאת כניסה לצוותים המיעון AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357880"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="266ae-102">שגיאת כניסה לצוותים המיעון AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="266ae-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="266ae-103">בעת הכניסה לצוותי Microsoft, ייתכן שתקבל את השגיאה: **מצטערים, אך יש לנו בעיה בחתימת החתימה שלך ב-AADSTS9000411: הבקשה אינה מעוצבת כראוי. הפרמטר "login_hint" משוכפל.**</span><span class="sxs-lookup"><span data-stu-id="266ae-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="266ae-104">כדי לטפל בבעיה זו, נא ודא שלקוחות צוותי Microsoft מתעדכנים.</span><span class="sxs-lookup"><span data-stu-id="266ae-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="266ae-105">לקבלת מידע נוסף אודות עדכון הלקוח, ראה [עדכון צוותי Microsoft](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="266ae-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="266ae-106">אם אין באפשרותך לעדכן את הלקוח מסיבה כלשהי, התנתקות הלקוח תנקה את רוב הנתונים המאוחסנים במטמון.</span><span class="sxs-lookup"><span data-stu-id="266ae-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="266ae-107">עם זאת, אם עדיין יש לך בעיות לאחר התנתקות/כניסה, צא מהקבוצות ובבקשה נקה את מטמון הלקוח על-ידי ביצוע הפעולות הבאות:</span><span class="sxs-lookup"><span data-stu-id="266ae-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="266ae-108">סגור את צוותי Microsoft.</span><span class="sxs-lookup"><span data-stu-id="266ae-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="266ae-109">עבור אל:%appdata%\ucet\mols\dute\n ומחק את כל הקבצים.</span><span class="sxs-lookup"><span data-stu-id="266ae-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="266ae-110">פתח מחדש את צוותי Microsoft.</span><span class="sxs-lookup"><span data-stu-id="266ae-110">Reopen Microsoft Teams.</span></span>
