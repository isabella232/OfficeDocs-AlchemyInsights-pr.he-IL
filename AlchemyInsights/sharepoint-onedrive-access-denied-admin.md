---
title: פתרון בעיות בהודעות שנדחו על-ידי Access
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758440"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="a0281-102">פתרון בעיות של הודעות שנדחו ב-Access במרכז ניהול Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="a0281-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="a0281-103">אם אתה מקבל הודעת גישה שנדחתה בעת ניסיון לגלוש אל מרכז ניהול Sharepoint/OneDrive, נא ודא שאתה [מקצה רשיון למשתמש](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="a0281-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="a0281-104">אם למשתמש יש רשיון, עליך גם לוודא [שהוקצו לו תפקיד מנהל](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) שיכול לגשת למרכזי הניהול.</span><span class="sxs-lookup"><span data-stu-id="a0281-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="a0281-105">בעיה זו עשויה להתרחש גם כאשר משתמש נמחק ונוצר מחדש עם אותו שם ראשי של משתמש (UPN).</span><span class="sxs-lookup"><span data-stu-id="a0281-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="a0281-106">החשבון החדש נוצר על-ידי שימוש בערך PUID (מזהה Passport ייחודי) אחר.</span><span class="sxs-lookup"><span data-stu-id="a0281-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="a0281-107">כשהמשתמש מנסה לגשת לאוסף אתרים או ל-OneDrive שלהם, למשתמש יש PUID שגוי.</span><span class="sxs-lookup"><span data-stu-id="a0281-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="a0281-108">תרחיש שני כולל סינכרון ספריות עם יחידה ארגונית של Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="a0281-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="a0281-109">אם משתמשים כבר החתימו ב-SharePoint ולאחר מכן מועברים ל-OU אחר ומסונכרנים מחדש עם SharePoint, הם עלולים להיתקל בבעיה זו.</span><span class="sxs-lookup"><span data-stu-id="a0281-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="a0281-110">כדי לפתור בעיה זו, עליך לשחזר את ה-UPN המקורי עם השלבים במאמר, [לשחזר משתמש ב-Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="a0281-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="a0281-111">הערה: אם מרכז OneDrive או SharePoint Admin אינו זמין למשתמשים מרובים שהיו בעבר גישה, ייתכן שקיימת בעיית שירות זמנית.</span><span class="sxs-lookup"><span data-stu-id="a0281-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="a0281-112">[בדוק את לוח המחוונים של תקינות השירות](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="a0281-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


