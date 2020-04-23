---
title: דואר אלקטרוני של זרימת עבודה אינו נשלח
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766134"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="816a7-102">דואר אלקטרוני של זרימת עבודה אינו נשלח עבור רשימה או ספריה של SharePoint</span><span class="sxs-lookup"><span data-stu-id="816a7-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="816a7-103">דואר אלקטרוני מזרימות עבודה אינם נשלחים לכל המשתמשים או למשתמשים מסוימים בלבד, או שאתה רואה את השגיאה **שהודעת הדואר האלקטרוני אינה יכולה להישלח. ודא שלדואר האלקטרוני יש נמען חוקי**.</span><span class="sxs-lookup"><span data-stu-id="816a7-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="816a7-104">בדוק אם המשתמש קיים בקבוצת ההרשאות ' **כל האנשים** ' (רשימת המידע של המשתמש) עבור אוסף אתרים זה.</span><span class="sxs-lookup"><span data-stu-id="816a7-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="816a7-105">לדוגמה, כתובת<tenant>URL ישירה<sitename>: https://. sharepoint.com/sites//_layouts/15/b. מחבר שיפגרפיד = 0</span><span class="sxs-lookup"><span data-stu-id="816a7-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="816a7-106">אם המשתמש אינו קיים, ודא שהמשתמש נחתם בעמוד.</span><span class="sxs-lookup"><span data-stu-id="816a7-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="816a7-107">אם זהו משתמש חיצוני, ודא שההזמנה שלהם התקבלה.</span><span class="sxs-lookup"><span data-stu-id="816a7-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="816a7-108">אם המשתמש קיים בקבוצת ההרשאות, ודא שכתובת הדואר האלקטרוני נכונה.</span><span class="sxs-lookup"><span data-stu-id="816a7-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="816a7-109">אם כתובת הדואר האלקטרוני של המשתמשים אינה מוגדרת כאן, צור התראה לדוגמה עבור אותו משתמש אשר מאלץ את הסינכרון של חשבון משתמש זה מפרופילי משתמשים של SharePoint לאוסף אתרים זה.</span><span class="sxs-lookup"><span data-stu-id="816a7-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="816a7-110">דואר אלקטרוני מזרימות עבודה נשלחים למנהלי אוספי האתרים אך לא למשתמשים אחרים ולראות את השגיאה **HTTP אסורה ל- <span>https:</span>/_vti_bin/client.xvc.sp.utilities.utility.sendemail**.</span><span class="sxs-lookup"><span data-stu-id="816a7-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="816a7-111">ראה [גישה נדחתה בעת שליחת הודעת דואר אלקטרוני לקבוצת SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="816a7-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="816a7-112">כמו כן, ודא שתכונת אוסף **ההרשאות של משתמש בגישה מוגבלת של הרשאת המשתמש** אינה פעילה.</span><span class="sxs-lookup"><span data-stu-id="816a7-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="816a7-113">נושאים קשורים</span><span class="sxs-lookup"><span data-stu-id="816a7-113">Related topics</span></span>
<span data-ttu-id="816a7-114">רוצה לנסות את Microsoft Flow ב-SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="816a7-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="816a7-115">צור זרימה</span><span class="sxs-lookup"><span data-stu-id="816a7-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="816a7-116">SharePoint וזרימה</span><span class="sxs-lookup"><span data-stu-id="816a7-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


