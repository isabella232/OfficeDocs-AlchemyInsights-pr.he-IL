---
title: בעיות ביצועים-SharePoint או OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771245"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="1009d-102">SharePoint או OneDrive איטיים, לא נגישים או שאינם זמינים עבור משתמשים מרובים</span><span class="sxs-lookup"><span data-stu-id="1009d-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="1009d-103">אם אתר OneDrive או SharePoint אינו זמין למשתמשים מרובים שהיו ברשותם גישה בעבר, ייתכן שקיימת בעיה של שירות זמני.</span><span class="sxs-lookup"><span data-stu-id="1009d-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="1009d-104">[בדוק את לוח המחוונים של תקינות השירות](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="1009d-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="1009d-105">**הוספה ורשיון של המשתמש**</span><span class="sxs-lookup"><span data-stu-id="1009d-105">**Add and license the user**</span></span>

<span data-ttu-id="1009d-106">ודא [שתקצה רשיונות למשתמשים ב-Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="1009d-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="1009d-107">**הקצאת הרשאות**</span><span class="sxs-lookup"><span data-stu-id="1009d-107">**Assign Permissions**</span></span>

<span data-ttu-id="1009d-108">אם למשתמש הוקצה רשיון של Sharepoint והוא עדיין מקבל הודעת גישה שנדחתה, ודא שהוקצה לה [רמת הרשאה מתאימה](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .</span><span class="sxs-lookup"><span data-stu-id="1009d-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="1009d-109">**שקול להשתמש בתכונה ' בקשת גישה '**</span><span class="sxs-lookup"><span data-stu-id="1009d-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="1009d-110">[התכונה ' בקשת גישה](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) ' מאפשרת לאנשים לבקש גישה לתוכן שאינו כולל כעת הרשאה לראות.</span><span class="sxs-lookup"><span data-stu-id="1009d-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="1009d-111">**אפשר סקריפט מותאם אישית עלול לגרום לבעיות של access שנדחו**</span><span class="sxs-lookup"><span data-stu-id="1009d-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="1009d-112">קיימים תרחישים מסוימים שבהם ייתכן שהתכונה ' *אפשר סקריפט מותאם אישית* ' מציגה גישה שנדחתה.</span><span class="sxs-lookup"><span data-stu-id="1009d-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="1009d-113">לקבלת רשימה של תכונות מושפעות, שיקולי אבטחה ויכולת להפוך את התכונה ללא זמינה.</span><span class="sxs-lookup"><span data-stu-id="1009d-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="1009d-114">בקר [באפשרות אפשר או מנע סקריפט מותאם אישית](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="1009d-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

