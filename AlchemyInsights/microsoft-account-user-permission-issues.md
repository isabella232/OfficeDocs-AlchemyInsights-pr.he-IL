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
ms.openlocfilehash: 59713231da25be441e7c05d788337e66bf17265a
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768802"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="42156-102">פתרון בעיות-משתמש לא נמצא בספריה</span><span class="sxs-lookup"><span data-stu-id="42156-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="42156-103">אם משתמשים מקבלים הודעת שגיאה "לא ניתן למצוא את המשתמש" בספריה, אנא נסה שוב כאשר סוג הנושא הוא משתמש לא בספריה.</span><span class="sxs-lookup"><span data-stu-id="42156-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="42156-104">ניתן להשלים את השלבים הבאים כדי לפתור את הבעיה.</span><span class="sxs-lookup"><span data-stu-id="42156-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="42156-105">ודא שהחשבון שקיבל את ההזמנה בדואר האלקטרוני הוא אותו חשבון המשמש לכניסה מאוחר יותר.</span><span class="sxs-lookup"><span data-stu-id="42156-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="42156-106">ודא שהמשתמש משתמש באותו חשבון כדי לקבל את ההזמנה ולהיכנס לאתר.</span><span class="sxs-lookup"><span data-stu-id="42156-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="42156-107">לקבלת מידע נוסף, ראה [כיצד לנהל כינויים</a> עבור חשבון Microsoft שלך כדי לנהל את הכניסה למשרד 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="42156-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="42156-108">דפדף לכל אתר (ים) שבו המשתמש מקבל את השגיאה.</span><span class="sxs-lookup"><span data-stu-id="42156-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="42156-109">הוסף/י/_layouts/15/l.sfipd/0 (בתוך המרכאות הכפולות) עד לסוף כתובת ה-URL של האתר.</span><span class="sxs-lookup"><span data-stu-id="42156-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="42156-110">דוגמה: https://Il__ "contoso">. sharepoint. com/_layouts/15/Emp_sos.fid = 0.</span><span class="sxs-lookup"><span data-stu-id="42156-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="42156-111">בחר את המשתמש מתוך הרשימה.</span><span class="sxs-lookup"><span data-stu-id="42156-111">Select the user from the list.</span></span>

- <span data-ttu-id="42156-112">לחץ על **הסר הרשאות משתמש** מרצועת הכלים.</span><span class="sxs-lookup"><span data-stu-id="42156-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="42156-113">הוסף בחזרה את המשתמש ושלח ממנו את ההזמנה למשתמש.</span><span class="sxs-lookup"><span data-stu-id="42156-113">Add back the User and Resend the invite to the user.</span></span>

