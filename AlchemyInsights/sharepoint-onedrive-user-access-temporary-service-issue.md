---
title: בעיות ביצועים-SharePoint או OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 880b2bdd7b74f4365bcbff73a709d42e72be0e3a
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36535176"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="5156f-102">SharePoint או OneDrive איטי, נגיש או אינו זמין עבור משתמשים מרובים</span><span class="sxs-lookup"><span data-stu-id="5156f-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="5156f-103">אם אתר OneDrive או SharePoint אינו זמין למשתמשים מרובים שהיה בעבר בעל גישה, ייתכן שקיימת בעיית שירות זמניים.</span><span class="sxs-lookup"><span data-stu-id="5156f-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="5156f-104">[בדוק את לוח המחוונים של תקינות השירות](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="5156f-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="5156f-105">**רשיון המשתמש ולהוסיף**</span><span class="sxs-lookup"><span data-stu-id="5156f-105">**Add and license the user**</span></span>

<span data-ttu-id="5156f-106">ודא שאתה [מקצה רשיונות המשתמשים ב- Office 365 עבור העסק](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="5156f-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


<span data-ttu-id="5156f-107">**הקצאת הרשאות**</span><span class="sxs-lookup"><span data-stu-id="5156f-107">**Assign Permissions**</span></span>

<span data-ttu-id="5156f-108">אם למשתמש זה הוקצה רשיון Sharepoint והוא עדיין מקבל הודעה שהגישה נדחתה, נא ודא שלהם את [רמת ההרשאה המתאימה](https://docs.microsoft.com/sharepoint/understanding-permission-levels) שהוקצתה.</span><span class="sxs-lookup"><span data-stu-id="5156f-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="5156f-109">**עליך לשקול את השימוש בתכונה בקשת גישה**</span><span class="sxs-lookup"><span data-stu-id="5156f-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="5156f-110">[התכונה בקשת גישה](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) מאפשר לאנשים לבקש גישה לתוכן אין כעת להם הרשאה לראות.</span><span class="sxs-lookup"><span data-stu-id="5156f-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="5156f-111">**אפשר בקובץ script מותאם אישית עלול לגרום בעיות גישה**</span><span class="sxs-lookup"><span data-stu-id="5156f-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="5156f-112">ישנם תרחישים מסוימים כאשר התכונה *אפשר בקובץ script מותאם אישית* עשוי להיות הצגת שהגישה נדחתה.</span><span class="sxs-lookup"><span data-stu-id="5156f-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="5156f-113">לקבלת רשימה של תכונות המושפעות, שיקולי אבטחה ואת היכולת להשבית את התכונה.</span><span class="sxs-lookup"><span data-stu-id="5156f-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="5156f-114">נא בקר ב- [אפשר או מנע בקובץ script מותאם אישית](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="5156f-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

