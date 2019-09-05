---
title: פתרון בעיות-משתמש לא נמצא בספריה
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754193"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="14317-102">פתרון בעיות-משתמש לא נמצא בספריה</span><span class="sxs-lookup"><span data-stu-id="14317-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="14317-103">אם משתמשים מקבלים הודעת שגיאה "לא ניתן למצוא את המשתמש" בספריה.</span><span class="sxs-lookup"><span data-stu-id="14317-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="14317-104">נא נסה שוב כאשר משתמש סוג הנושא אינו בספריה.</span><span class="sxs-lookup"><span data-stu-id="14317-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="14317-105">ניתן להשלים את השלבים הבאים כדי לפתור את הבעיה.</span><span class="sxs-lookup"><span data-stu-id="14317-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="14317-106">ודא שהחשבון שקיבל את ההזמנה בדואר האלקטרוני הוא אותו חשבון המשמש לכניסה מאוחר יותר.</span><span class="sxs-lookup"><span data-stu-id="14317-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="14317-107">ודא שהמשתמש משתמש באותו חשבון כדי לקבל את ההזמנה ולהיכנס לאתר.</span><span class="sxs-lookup"><span data-stu-id="14317-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="14317-108">לקבלת מידע נוסף, ראה [כיצד לנהל כינויים</a> עבור חשבון Microsoft שלך כדי לנהל את הכניסה למשרד 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="14317-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="14317-109">דפדף לכל אתר (ים) שבו המשתמש מקבל את השגיאה.</span><span class="sxs-lookup"><span data-stu-id="14317-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="14317-110">הוסף את המילה "/_layouts/15/people.aspx/membershipgroupid = 0" (בתוך המרכאות הכפולות) עד לסוף כתובת ה-URL של האתר.</span><span class="sxs-lookup"><span data-stu-id="14317-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="14317-111">דוגמה: https://< _ "contoso">. sharepoint. com/_ פריסות/15/אנשים. aspx/מחבר שיפגרפיד = 0.</span><span class="sxs-lookup"><span data-stu-id="14317-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="14317-112">בחר את המשתמש מתוך הרשימה.</span><span class="sxs-lookup"><span data-stu-id="14317-112">Select the user from the list.</span></span>

- <span data-ttu-id="14317-113">לחץ על **הסר הרשאות משתמש** מרצועת הכלים.</span><span class="sxs-lookup"><span data-stu-id="14317-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="14317-114">הוסף בחזרה את המשתמש ושלח ממנו את ההזמנה למשתמש.</span><span class="sxs-lookup"><span data-stu-id="14317-114">Add back the User and Resend the invite to the user.</span></span>

