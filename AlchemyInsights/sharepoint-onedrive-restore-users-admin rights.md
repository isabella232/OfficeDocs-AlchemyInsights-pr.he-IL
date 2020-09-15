---
title: פתרון בעיות גישה שנדחו על-ידי הודעות לאתרי OneDrive for Business
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670617"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="33389-102">פתרון בעיות גישה שנדחו על-ידי הודעות לאתרי OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="33389-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="33389-103">בעיה זו מתרחשת לעתים קרובות, כאשר משתמש נמחק ונוצר מחדש באמצעות אותו שם ראשי של המשתמש (UPN).</span><span class="sxs-lookup"><span data-stu-id="33389-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="33389-104">החשבון החדש נוצר באמצעות ערך שונה של PUID (מזהה ייחודי של Passport).</span><span class="sxs-lookup"><span data-stu-id="33389-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="33389-105">כאשר המשתמש מנסה לגשת לאוסף אתרים או לOneDrive שלו, למשתמש יש PUID שגוי.</span><span class="sxs-lookup"><span data-stu-id="33389-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="33389-106">תרחיש נוסף כולל סינכרון מדריכי כתובות עם יחידה ארגונית של Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="33389-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="33389-107">אם המשתמשים כבר נכנסו ל-SharePoint ולאחר מכן מועברים ל-OU אחר ומסונכרנים מחדש ב-SharePoint, הם עשויים להיתקל בבעיה זו.</span><span class="sxs-lookup"><span data-stu-id="33389-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="33389-108">כדי לפתור בעיה זו, עליך לשחזר את ה-UPN המקורי בשלבים המפורטים במאמר, [לשחזר משתמש ב-Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="33389-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="33389-109">אם אין באפשרותך לשחזר את המשתמש המקורי, עליך להסיר את המשתמש הישן מאתר OneDrive באמצעות שלבים אלה, [להסיר משתמש מרשימת פרטי המשתמש]().</span><span class="sxs-lookup"><span data-stu-id="33389-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="33389-110">לאחר ביצוע פעולה זו, באפשרותך לוודא שלמשתמש יש זכויות מנהל מערכת לאתר OneDrive על-ידי ביצוע השלבים [להוספת מנהל מערכת עבור OneDrive של משתמש](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="33389-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="33389-111">לקבלת מידע נוסף אודות רמות הרשאה, עיין במאמר [הכרת רמות הרשאה ב-SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="33389-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
