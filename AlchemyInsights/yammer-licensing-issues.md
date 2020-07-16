---
title: בעיות רישוי של יממר
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148240"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="60d7c-102">בעיות רישוי של יממר</span><span class="sxs-lookup"><span data-stu-id="60d7c-102">Yammer licensing issues</span></span>

<span data-ttu-id="60d7c-103">על כל המשתמשים להיות בעלי רשיון כדי להשתמש בשירות ארגון Yammer, אך כברירת מחדל, Yammer אינו מחייב שלמשתמשים יהיה רשיון לגשת לשירות.</span><span class="sxs-lookup"><span data-stu-id="60d7c-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="60d7c-104">כאשר מנהל מערכת משנה את ההגדרה כדי לחסום את Microsoft 365 משתמשים ללא רשיונות של Yammer, משתמשים שאינם מוקצים לרשיון Enterprise של Yammer לא יוכלו לגשת לשירות Yammer.</span><span class="sxs-lookup"><span data-stu-id="60d7c-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="60d7c-105">לקבלת מידע נוסף, ראה [ניהול רשיונות משתמש של Yammer ב-Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="60d7c-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="60d7c-106">כאשר רשיונות מוסרים מהמשתמשים, האריח Yammer אינו מוצג עוד, ושירותים אחרים יכולים להשתמש בהסרת רשיון כדי להסתיר תכונות.</span><span class="sxs-lookup"><span data-stu-id="60d7c-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="60d7c-107">במקרים אחרים, תכונות עדיין יכולות להופיע אך דורשות הקצאת רשיון להפעלה.</span><span class="sxs-lookup"><span data-stu-id="60d7c-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="60d7c-108">**הרשיון אינו מקבל עדכון עבור המשתמש**</span><span class="sxs-lookup"><span data-stu-id="60d7c-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="60d7c-109">לעיתים, מוקצה למשתמש רשיון אך עדיין אין לו אפשרות לגשת ליאממר.</span><span class="sxs-lookup"><span data-stu-id="60d7c-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="60d7c-110">סביר יותר שעיכובים יתרחשו כאשר מתבצעת הקצאת רשיון המונים.</span><span class="sxs-lookup"><span data-stu-id="60d7c-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="60d7c-111">ייתכן שמשתמשי יאמר לא יעודכנו באותו סדר שבו משתנים רשיונות בתכלת לספירה כיוון שהמערכת פועלת באופן אסינכרוני.</span><span class="sxs-lookup"><span data-stu-id="60d7c-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="60d7c-112">המתן עד 24 שעות לפני פתיחת אירוע תמיכה כדי לדווח על בעיות בסינכרון רשיונות.</span><span class="sxs-lookup"><span data-stu-id="60d7c-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="60d7c-113">**הקצאת רשיון בצובר**</span><span class="sxs-lookup"><span data-stu-id="60d7c-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="60d7c-114">רשיונות ניתן להקצות באמצעות מרכז הניהול או scripting PowerShell.</span><span class="sxs-lookup"><span data-stu-id="60d7c-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="60d7c-115">לקבלת מידע נוסף, ראה [הקצאת רשיונות למשתמשים](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) [והקצאת רשיונות לחשבונות משתמשים באמצעות Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="60d7c-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="60d7c-116">התמיכה של Microsoft אינה מספקת סיוע ביצירת קבצי script, אך התיעוד בהקצאת רשיון של Yammer זמין.</span><span class="sxs-lookup"><span data-stu-id="60d7c-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="60d7c-117">לקבלת מידע נוסף, ראה [ניהול רשיונות Yammer באמצעות Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="60d7c-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>