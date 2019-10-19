---
title: בעיות ביצועים-SharePoint או OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 7e218cfff81274cd16d55dec2c5243eb8b74a3b7
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750557"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="7129c-102">SharePoint או OneDrive איטי, לא נגיש או לא זמין עבור משתמשים מרובים</span><span class="sxs-lookup"><span data-stu-id="7129c-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="7129c-103">אם אתר OneDrive או SharePoint אינו זמין למשתמשים מרובים שהיו בעבר גישה, ייתכן שקיימת בעיית שירות זמנית.</span><span class="sxs-lookup"><span data-stu-id="7129c-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="7129c-104">[בדוק את לוח המחוונים של תקינות השירות](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="7129c-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="7129c-105">**הוסף רישיון למשתמש**</span><span class="sxs-lookup"><span data-stu-id="7129c-105">**Add and license the user**</span></span>

<span data-ttu-id="7129c-106">ודא שאתה [מקצה רשיונות למשתמשים ב-Office 365 עבור עסקים](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="7129c-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


<span data-ttu-id="7129c-107">**הקצאת הרשאות**</span><span class="sxs-lookup"><span data-stu-id="7129c-107">**Assign Permissions**</span></span>

<span data-ttu-id="7129c-108">אם המשתמש הוקצה לרשיון של Sharepoint ועדיין מקבל הודעה שנדחתה על-ידי הגישה, ודא שהוקצתה להם [רמת ההרשאה המתאימה](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .</span><span class="sxs-lookup"><span data-stu-id="7129c-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="7129c-109">**שקול להשתמש בתכונת בקשת הגישה**</span><span class="sxs-lookup"><span data-stu-id="7129c-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="7129c-110">[תכונת בקשת הגישה](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) מאפשרת לאנשים לבקש גישה לתוכן שאין להם כרגע הרשאה לראותם.</span><span class="sxs-lookup"><span data-stu-id="7129c-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="7129c-111">**אפשר קובץ script מותאם אישית עלול לגרום לבעיות שנדחו על-ידי גישה**</span><span class="sxs-lookup"><span data-stu-id="7129c-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="7129c-112">קיימים תרחישים מסוימים בהם ייתכן שתכונת *הסקריפט המותאם אישית* מציגה גישה שנדחתה.</span><span class="sxs-lookup"><span data-stu-id="7129c-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="7129c-113">לקבלת רשימה של תכונות מושפעות, שיקולי אבטחה והיכולת להשבית את התכונה.</span><span class="sxs-lookup"><span data-stu-id="7129c-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="7129c-114">בקר [באפשרות אפשר או מנע script מותאם אישית](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="7129c-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

