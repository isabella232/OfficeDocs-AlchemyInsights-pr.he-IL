---
title: פתרון בעיות בהודעות של Access שנדחו
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767663"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="004d0-102">פתרון בעיות בהודעות של Access שנדחו במרכז הניהול של Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="004d0-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="004d0-103">אם אתה מקבל הודעת גישה שנדחתה בעת ניסיון לנווט למרכז הניהול של Sharepoint/OneDrive, ודא שאתה [מקצה רשיון למשתמש](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="004d0-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="004d0-104">אם למשתמש יש רשיון, עליך גם לוודא שהוא [מוקצה לתפקיד מנהל מערכת](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) שיכול לגשת למרכזי הניהול.</span><span class="sxs-lookup"><span data-stu-id="004d0-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="004d0-105">בעיה זו עלולה להתרחש גם כאשר משתמש נמחק ונוצר מחדש עם אותו שם ראשי של המשתמש (UPN).</span><span class="sxs-lookup"><span data-stu-id="004d0-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="004d0-106">החשבון החדש נוצר באמצעות ערך שונה של PUID (מזהה ייחודי של Passport).</span><span class="sxs-lookup"><span data-stu-id="004d0-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="004d0-107">כאשר המשתמש מנסה לגשת לאוסף אתרים או לOneDrive שלו, למשתמש יש PUID שגוי.</span><span class="sxs-lookup"><span data-stu-id="004d0-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="004d0-108">תרחיש נוסף כולל סינכרון מדריכי כתובות עם יחידה ארגונית של Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="004d0-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="004d0-109">אם המשתמשים כבר נכנסו ל-SharePoint ולאחר מכן מועברים ל-OU אחר ומסונכרנים מחדש ב-SharePoint, הם עשויים להיתקל בבעיה זו.</span><span class="sxs-lookup"><span data-stu-id="004d0-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="004d0-110">כדי לפתור בעיה זו, עליך לשחזר את ה-UPN המקורי בשלבים המפורטים במאמר, [לשחזר משתמש ב-Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="004d0-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="004d0-111">הערה: אם מרכז הניהול של OneDrive או SharePoint אינו זמין למשתמשים מרובים שהיו ברשותם גישה בעבר, ייתכן שקיימת בעיה של שירות זמני.</span><span class="sxs-lookup"><span data-stu-id="004d0-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="004d0-112">[בדוק את לוח המחוונים של תקינות השירות](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="004d0-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


