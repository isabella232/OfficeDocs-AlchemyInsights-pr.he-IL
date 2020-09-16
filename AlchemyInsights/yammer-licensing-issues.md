---
title: בעיות רישוי של קטרת
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657277"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="b21f4-102">בעיות רישוי של קטרת</span><span class="sxs-lookup"><span data-stu-id="b21f4-102">Yammer licensing issues</span></span>

<span data-ttu-id="b21f4-103">כל המשתמשים חייבים להיות בעלי רשיון לשימוש בשירות Enterprise קטרת, אך כברירת מחדל, קטרת אינו מחייב שלמשתמשים יהיה רשיון לגשת לשירות.</span><span class="sxs-lookup"><span data-stu-id="b21f4-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="b21f4-104">כאשר מנהל מערכת משנה את ההגדרה כדי לחסום את משתמשי Microsoft 365 ללא רשיונות קטרת, המשתמשים לא הקצו לרשיון של קטרת Enterprise אין גישה לשירות קטרת.</span><span class="sxs-lookup"><span data-stu-id="b21f4-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="b21f4-105">לקבלת מידע נוסף, ראה [ניהול רשיונות משתמשים של קטרת ב-Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="b21f4-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="b21f4-106">בעת הסרת רשיונות ממשתמשים, האריח של קטרת אינו מוצג עוד ושירותים אחרים יכולים להשתמש בהסרת רשיונות כדי להסתיר תכונות.</span><span class="sxs-lookup"><span data-stu-id="b21f4-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="b21f4-107">במקרים אחרים, תכונות עדיין יכולות להופיע אך נדרשת הקצאת רשיון להפעלה.</span><span class="sxs-lookup"><span data-stu-id="b21f4-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="b21f4-108">**הרשיון אינו מתעדכן עבור המשתמש**</span><span class="sxs-lookup"><span data-stu-id="b21f4-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="b21f4-109">לעתים, למשתמש מוקצה רשיון, אך עדיין אינו מצליח לגשת ל-קטרת.</span><span class="sxs-lookup"><span data-stu-id="b21f4-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="b21f4-110">סביר להניח שהעיכובים מתרחשים כאשר הקצאת רשיון המונים מתבצעת.</span><span class="sxs-lookup"><span data-stu-id="b21f4-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="b21f4-111">ייתכן שמשתמשי קטרת לא יתעדכנו באותו הסדר שבו הרשיונות משתנים בתכלת לספירה מכיוון שהמערכת פועלת באופן אסינכרוני.</span><span class="sxs-lookup"><span data-stu-id="b21f4-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="b21f4-112">המתן עד 24 שעות לפני פתיחת מקרה תמיכה כדי לדווח על בעיות סינכרון רשיונות.</span><span class="sxs-lookup"><span data-stu-id="b21f4-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="b21f4-113">**הקצאת רשיון בצובר**</span><span class="sxs-lookup"><span data-stu-id="b21f4-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="b21f4-114">ניתן להקצות רשיונות באמצעות הסקריפטים של מרכז הניהול או של PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b21f4-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="b21f4-115">לקבלת מידע נוסף, ראה [הקצאת רשיונות למשתמשים](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) [והקצאת רשיונות לחשבונות משתמשים באמצעות Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="b21f4-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="b21f4-116">התמיכה של Microsoft אינה מספקת סיוע ביצירת קבצי script, אך התיעוד על הקצאת רשיון של קטרת זמין.</span><span class="sxs-lookup"><span data-stu-id="b21f4-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="b21f4-117">לקבלת מידע נוסף, ראה [ניהול רשיונות קטרת באמצעות Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="b21f4-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>