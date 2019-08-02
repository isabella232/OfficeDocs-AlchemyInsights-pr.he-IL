---
title: זרימת דואר אלקטרוני לא נשלחת
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 783bf0a5721aa5db7088432c71e06cac6dc90513
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059605"
---
# <a name="workflow-email-is-not-being-sent"></a><span data-ttu-id="e4bea-102">זרימת דואר אלקטרוני לא נשלחת</span><span class="sxs-lookup"><span data-stu-id="e4bea-102">Workflow email is not being sent</span></span>

1. <span data-ttu-id="e4bea-103">דואר אלקטרוני מתוך זרימות עבודה אינן נשלחות לכל המשתמשים או רק למשתמשים מסוימים, או שאתה רואה שאין אפשרות לשלוח את השגיאה **הודעת הדואר האלקטרוני. ודא כי הדואר האלקטרוני יש נמען חוקי**.</span><span class="sxs-lookup"><span data-stu-id="e4bea-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

<span data-ttu-id="e4bea-104">בדוק אם המשתמש קיים בקבוצה הרשאות **לכל האנשים** (רשימת פרטי משתמש) עבור אוסף אתרים זה.</span><span class="sxs-lookup"><span data-stu-id="e4bea-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="e4bea-105">דגימה ישירה של כתובת URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="e4bea-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

- <span data-ttu-id="e4bea-106">אם המשתמש אינו קיים, ודא שהמשתמש מחובר לתוך הדף.</span><span class="sxs-lookup"><span data-stu-id="e4bea-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
- <span data-ttu-id="e4bea-107">אם הוא משתמש חיצוני, ודא כי ההזמנה שלהם התקבלה.</span><span class="sxs-lookup"><span data-stu-id="e4bea-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
- <span data-ttu-id="e4bea-108">אם המשתמש קיים בקבוצה הרשאות, ודא כי כתובת דואר אלקטרוני נכונה.</span><span class="sxs-lookup"><span data-stu-id="e4bea-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
- <span data-ttu-id="e4bea-109">אם כתובת הדואר האלקטרוני של משתמשים לא מוגדר כאן, צור בדוגמה של התראה עבור משתמש זה שכופה על הסינכרון של חשבון משתמש זה מפרופילי המשתמש של SharePoint כדי באוסף אתרים זה.</span><span class="sxs-lookup"><span data-stu-id="e4bea-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="e4bea-110">דואר אלקטרוני מזרימות נשלחות המנהלים של אוספי אתרים אך לא משתמשים אחרים ולראות את השגיאה \*\*HTTP אסור כדי <spam> <spam> \*\* <spam> <spam>.</span><span class="sxs-lookup"><span data-stu-id="e4bea-110">Email from Workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <spam><spam>https://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**<spam><spam>.</span></span>
 

<span data-ttu-id="e4bea-111">ראה [Access נדחתה כאשר דואר אלקטרוני שנשלחו אל קבוצות](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="e4bea-111">See [Access Denied when sent email to groups](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span></span>

<span data-ttu-id="e4bea-112">כמו כן, ודא כי תכונה **מצב נעילה של הרשאת משתמש גישה מוגבלת** של אוסף אתרים אינו פעיל.</span><span class="sxs-lookup"><span data-stu-id="e4bea-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>

## <a name="related-topics"></a><span data-ttu-id="e4bea-113">נושאים קשורים</span><span class="sxs-lookup"><span data-stu-id="e4bea-113">Related topics</span></span>
- [<span data-ttu-id="e4bea-114">צור זרימה</span><span class="sxs-lookup"><span data-stu-id="e4bea-114">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="e4bea-115">SharePoint וזרימה</span><span class="sxs-lookup"><span data-stu-id="e4bea-115">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


