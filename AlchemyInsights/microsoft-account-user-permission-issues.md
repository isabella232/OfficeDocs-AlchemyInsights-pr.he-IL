---
title: פתרון בעיות-המשתמש לא נמצא במדריך כתובות
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725408"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="d5cd4-102">פתרון בעיות-המשתמש לא נמצא במדריך כתובות</span><span class="sxs-lookup"><span data-stu-id="d5cd4-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="d5cd4-103">אם המשתמשים מקבלים הודעת שגיאה "לא ניתן למצוא את המשתמש" במדריך הכתובות, נסה שוב כאשר סוג הבעיה אינו מופיע במדריך הכתובות.</span><span class="sxs-lookup"><span data-stu-id="d5cd4-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="d5cd4-104">ניתן להשלים את השלבים הבאים כדי לפתור את הבעיה.</span><span class="sxs-lookup"><span data-stu-id="d5cd4-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="d5cd4-105">ודא שהחשבון שקיבל את ההזמנה לדואר אלקטרוני הוא אותו חשבון שנעשה בו שימוש כדי להיכנס במועד מאוחר יותר.</span><span class="sxs-lookup"><span data-stu-id="d5cd4-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="d5cd4-106">ודא שהמשתמש משתמש באותו חשבון כדי לקבל את ההזמנה ולהיכנס לאתר.</span><span class="sxs-lookup"><span data-stu-id="d5cd4-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="d5cd4-107">לקבלת מידע נוסף, ראה [כיצד לנהל כינויים עבור חשבון Microsoft שלך </a> כדי לנהל את הכניסה של microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="d5cd4-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="d5cd4-108">אתר את כל האתרים שבהם המשתמש מקבל את השגיאה.</span><span class="sxs-lookup"><span data-stu-id="d5cd4-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="d5cd4-109">הוסף את "/_layouts/15/people.aspx/membershipgroupid = 0" (בתוך המרכאות הכפולות) עד סוף כתובת ה-URL של האתר.</span><span class="sxs-lookup"><span data-stu-id="d5cd4-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="d5cd4-110">דוגמה: https://< "contoso">. sharepoint. com/_layouts/15/people.aspx/membershipGroupId = 0.</span><span class="sxs-lookup"><span data-stu-id="d5cd4-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="d5cd4-111">בחר את המשתמש מהרשימה.</span><span class="sxs-lookup"><span data-stu-id="d5cd4-111">Select the user from the list.</span></span>

- <span data-ttu-id="d5cd4-112">לחץ על **הסר הרשאות משתמש** מרצועת הכלים.</span><span class="sxs-lookup"><span data-stu-id="d5cd4-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="d5cd4-113">הוסף את המשתמש ושלח אותו מחדש למשתמש.</span><span class="sxs-lookup"><span data-stu-id="d5cd4-113">Add back the User and Resend the invite to the user.</span></span>

