---
title: הדואר האלקטרוני של זרימת העבודה אינו נשלח
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748990"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="0e399-102">הדואר האלקטרוני של זרימת העבודה אינו נשלח עבור רשימה או ספריה של SharePoint</span><span class="sxs-lookup"><span data-stu-id="0e399-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="0e399-103">דואר אלקטרוני מזרימות עבודה אינו נשלח לכל המשתמשים או רק למשתמשים ספציפיים, או שאתה רואה את השגיאה **אין אפשרות לשלוח את הודעת הדואר האלקטרוני. ודא שהדואר האלקטרוני מכיל נמען חוקי**.</span><span class="sxs-lookup"><span data-stu-id="0e399-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="0e399-104">בדוק אם המשתמש קיים בקבוצת ההרשאות ' **כל האנשים** ' (רשימת פרטי משתמש) עבור אוסף אתרים זה.</span><span class="sxs-lookup"><span data-stu-id="0e399-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="0e399-105">כתובת URL ישירה <tenant> לדוגמה: https://. sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="0e399-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="0e399-106">אם המשתמש אינו קיים, ודא שהמשתמש מחובר לעמוד.</span><span class="sxs-lookup"><span data-stu-id="0e399-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="0e399-107">אם זהו משתמש חיצוני, ודא שההזמנה שלהם התקבלה.</span><span class="sxs-lookup"><span data-stu-id="0e399-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="0e399-108">אם המשתמש קיים בקבוצה הרשאות, ודא שכתובת הדואר האלקטרוני נכונה.</span><span class="sxs-lookup"><span data-stu-id="0e399-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="0e399-109">אם כתובת הדואר האלקטרוני של המשתמשים אינה מוגדרת כאן, צור התראה לדוגמה עבור משתמש זה, הכופה את הסינכרון של חשבון משתמש זה מפרופילי משתמשים של SharePoint לאוסף אתרים זה.</span><span class="sxs-lookup"><span data-stu-id="0e399-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="0e399-110">דואר אלקטרוני מזרימות עבודה נשלח למנהלי אוסף האתרים אך לא למשתמשים אחרים ולראות את השגיאה **HTTP אסור ל <span>-https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.sendemail**.</span><span class="sxs-lookup"><span data-stu-id="0e399-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="0e399-111">ראה [Access נדחה כאשר אתה שולח הודעת דואר אלקטרוני לקבוצת SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="0e399-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="0e399-112">כמו כן, ודא שהתכונה ' אוסף אתרים ' של **' מצב נעילה ' של הרשאת משתמשים בעלת גישה מוגבלת** אינה פעילה.</span><span class="sxs-lookup"><span data-stu-id="0e399-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="0e399-113">נושאים קשורים</span><span class="sxs-lookup"><span data-stu-id="0e399-113">Related topics</span></span>
<span data-ttu-id="0e399-114">מעוניין לנסות את Microsoft Flow ב-SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="0e399-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="0e399-115">יצירת זרימה</span><span class="sxs-lookup"><span data-stu-id="0e399-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="0e399-116">SharePoint ו-Flow</span><span class="sxs-lookup"><span data-stu-id="0e399-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


