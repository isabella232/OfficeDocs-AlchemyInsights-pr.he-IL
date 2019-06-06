---
title: פתרון בעיות של הודעות נדחתה על-ידי Access
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 5958ad06ca905f713b5f56aa5c536e95a485f01c
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735739"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="5e02d-102">פתרון בעיות של הודעות נדחתה על-ידי Access</span><span class="sxs-lookup"><span data-stu-id="5e02d-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="5e02d-103">אם אתה מקבל הודעה שהגישה נדחתה בעת ניסיון גלישה באתר Sharepoint מקוונת, נא ראה המאמרים להלן.</span><span class="sxs-lookup"><span data-stu-id="5e02d-103">If you are receiving an access denied message when attempting to browse a Sharepoint Online site, please see the below articles.</span></span>

## <a name="add-and-license-the-user"></a><span data-ttu-id="5e02d-104">רשיון המשתמש ולהוסיף</span><span class="sxs-lookup"><span data-stu-id="5e02d-104">Add and License the user</span></span>

<span data-ttu-id="5e02d-105">ודא שאתה [מקצה רשיונות המשתמשים ב- Office 365 עבור העסק](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="5e02d-105">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>

<span data-ttu-id="5e02d-106">הקצאת הרשאות</span><span class="sxs-lookup"><span data-stu-id="5e02d-106">Assign Permissions</span></span>

<span data-ttu-id="5e02d-107">אם למשתמש זה הוקצה רשיון Sharepoint והוא עדיין מקבל הודעה שהגישה נדחתה, נא ודא שלהם את [רמת ההרשאה המתאימה שהוקצתה](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="5e02d-107">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level assigned](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span></span>

<span data-ttu-id="5e02d-108">עליך לשקול את השימוש בתכונה בקשת גישה</span><span class="sxs-lookup"><span data-stu-id="5e02d-108">Consider using the access request feature</span></span>

<span data-ttu-id="5e02d-109">התכונה [בקשת גישה](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) מאפשר לאנשים לבקש גישה לתוכן אין כעת להם הרשאה לראות.</span><span class="sxs-lookup"><span data-stu-id="5e02d-109">The [access request](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) feature allows people to request access to content that they do not currently have permission to see.</span></span> 

<span data-ttu-id="5e02d-110">אפשר בקובץ script מותאם אישית עלול לגרום בעיות גישה</span><span class="sxs-lookup"><span data-stu-id="5e02d-110">Allow custom script may cause access denied issues</span></span>

<span data-ttu-id="5e02d-111">ישנם תרחישים מסוימים שבהם התכונה "אפשר בקובץ script מותאם אישית" עשוי להיות הצגת שהגישה נדחתה.</span><span class="sxs-lookup"><span data-stu-id="5e02d-111">There are certain scenarios where the "Allow custom script" feature may be presenting an access denied.</span></span> <span data-ttu-id="5e02d-112">לקבלת רשימה של תכונות המושפעות, שיקולי אבטחה ואת היכולת להשבית את התכונה.</span><span class="sxs-lookup"><span data-stu-id="5e02d-112">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="5e02d-113">נא בקר, [אפשר או מנע בקובץ script מותאם אישית](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="5e02d-113">Please visit , [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script)</span></span>

<span data-ttu-id="5e02d-114">הערה: אם אתר OneDrive או SharePoint אינו זמין למשתמשים מרובים שהיה בעבר בעל גישה, ייתכן שישנה בעיה בשירות זמניים.</span><span class="sxs-lookup"><span data-stu-id="5e02d-114">Note: If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="5e02d-115">[בדוק את לוח המחוונים של תקינות השירות](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="5e02d-115">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


  

