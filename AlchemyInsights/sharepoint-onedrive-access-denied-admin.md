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
ms.openlocfilehash: 0a885e15d54c9337711f2528628789dfcb903264
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36503529"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="08421-102">פתרון בעיות של הודעות נדחתה על-ידי Access במרכז הניהול של Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="08421-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="08421-103">אם אתה מקבל הודעה שהגישה נדחתה בעת ניסיון לבצע עיון למרכז הניהול של Sharepoint/OneDrive, נא ודא כי זה [רשיון למשתמש הקצה](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="08421-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="08421-104">אם למשתמש יש רשיון, עליך לוודא גם שהם [להקצות תפקיד מנהל](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) יכולים לגשת אליהם מרכזי admin.</span><span class="sxs-lookup"><span data-stu-id="08421-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="08421-105">בעיה זו עלולה להתרחש גם כאשר המשתמש יימחק וייווצר מחדש עם אותו השם העיקרי של המשתמש (UPN).</span><span class="sxs-lookup"><span data-stu-id="08421-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="08421-106">החשבון החדש נוצר באמצעות ערך ה-PUID (מזהה ייחודי של Passport) שונה.</span><span class="sxs-lookup"><span data-stu-id="08421-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="08421-107">כאשר המשתמש מנסה לגשת לאוסף אתרים או OneDrive שלהם, יש למשתמש של ה-PUID שגוי.</span><span class="sxs-lookup"><span data-stu-id="08421-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="08421-108">תרחיש השני כרוך סינכרון ספריות עם יחידה ארגונית של Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="08421-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="08421-109">אם יש כבר נכנסו ל- SharePoint, ולאחר מכן הם הועברו לתפריט OU שונים ומשתמשים resynced עם SharePoint, עלול להיתקל בבעיה זו.</span><span class="sxs-lookup"><span data-stu-id="08421-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="08421-110">כדי לפתור בעיה זו, שחזר את UPN המקורי עם השלבים במאמר, [שחזור משתמש ב- Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="08421-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="08421-111">הערה: אם מרכז OneDrive או הניהול של SharePoint אינו זמין למשתמשים מרובים שהיה בעבר בעל גישה, ייתכן שקיימת בעיית שירות זמניים.</span><span class="sxs-lookup"><span data-stu-id="08421-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="08421-112">[בדוק את לוח המחוונים של תקינות השירות](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="08421-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


