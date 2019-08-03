---
title: פתרון הבעיה - המשתמש לא נמצא בספריה
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0909edc581c811fdc4683b004e0df0adbac88d1c
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/26/2019
ms.locfileid: "35249914"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="ab29a-102">פתרון הבעיה - המשתמש לא נמצא בספריה</span><span class="sxs-lookup"><span data-stu-id="ab29a-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="ab29a-103">אם משתמשים מקבלים שגיאה הודעת "המשתמש לא נמצא' בספריה.</span><span class="sxs-lookup"><span data-stu-id="ab29a-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="ab29a-104">נא נסה שוב כאשר סוג הבעיה אינו משתמש בספריה.</span><span class="sxs-lookup"><span data-stu-id="ab29a-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="ab29a-105">יש להשלים את השלבים הבאים כדי לפתור את הבעיה.</span><span class="sxs-lookup"><span data-stu-id="ab29a-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="ab29a-106">ודא שהחשבון קיבל שההזמנה בדוא ל הוא באותו חשבון אשר משמש להיכנס במועד מאוחר יותר.</span><span class="sxs-lookup"><span data-stu-id="ab29a-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="ab29a-107">ודא כי המשתמש עושה שימוש באותו החשבון כדי לקבל את ההזמנה או להיכנס אל האתר.</span><span class="sxs-lookup"><span data-stu-id="ab29a-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="ab29a-108">לקבלת מידע נוסף, ראה [כיצד לנהל כינויים עבור חשבון Microsoft שלך</a> כדי לנהל את הכניסה Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="ab29a-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="ab29a-109">דפדף אל כל אתרים שבו המשתמש מקבל את השגיאה.</span><span class="sxs-lookup"><span data-stu-id="ab29a-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="ab29a-110">הוספת "/ _layouts/15/people.aspx/membershipgroupid=0" (בתוך מרכאות כפולות) לסוף כתובת ה-URL של האתר.</span><span class="sxs-lookup"><span data-stu-id="ab29a-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="ab29a-111">דוגמה: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="ab29a-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="ab29a-112">בחר את המשתמש מתוך הרשימה.</span><span class="sxs-lookup"><span data-stu-id="ab29a-112">Select the user from the list.</span></span>

- <span data-ttu-id="ab29a-113">לחץ על **הסר הרשאות משתמש** מרצועת הכלים.</span><span class="sxs-lookup"><span data-stu-id="ab29a-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="ab29a-114">הוסף את המשתמש ושלח את ההזמנה למשתמש.</span><span class="sxs-lookup"><span data-stu-id="ab29a-114">Add back the User and Resend the invite to the user.</span></span>

