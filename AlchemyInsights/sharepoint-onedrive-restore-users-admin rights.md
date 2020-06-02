---
title: פתרון בעיות ב-Access דחה הודעות ל-OneDrive עבור אתרים עסקיים
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511185"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="82d81-102">פתרון בעיות ב-Access דחה הודעות ל-OneDrive עבור אתרים עסקיים</span><span class="sxs-lookup"><span data-stu-id="82d81-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="82d81-103">בעיה זו מתרחשת לעתים קרובות כאשר משתמש נמחק ונוצר מחדש עם אותו שם ראשי של משתמש (UPN).</span><span class="sxs-lookup"><span data-stu-id="82d81-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="82d81-104">החשבון החדש נוצר על-ידי שימוש בערך PUID (מזהה Passport ייחודי) אחר.</span><span class="sxs-lookup"><span data-stu-id="82d81-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="82d81-105">כשהמשתמש מנסה לגשת לאוסף אתרים או ל-OneDrive שלהם, למשתמש יש PUID שגוי.</span><span class="sxs-lookup"><span data-stu-id="82d81-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="82d81-106">תרחיש שני כולל סינכרון ספריות עם יחידה ארגונית של Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="82d81-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="82d81-107">אם משתמשים כבר החתימו ב-SharePoint ולאחר מכן מועברים ל-OU אחר ומסונכרנים מחדש עם SharePoint, הם עלולים להיתקל בבעיה זו.</span><span class="sxs-lookup"><span data-stu-id="82d81-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="82d81-108">כדי לפתור בעיה זו עליך לשחזר את ה-UPN המקורי עם השלבים במאמר, [לשחזר משתמש ב-Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="82d81-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="82d81-109">אם אין באפשרותך לשחזר את המשתמש המקורי, עליך להסיר את המשתמש הישן מהאתר OneDrive באמצעות שלבים אלה, [להסיר משתמש מרשימת פרטי המשתמש]().</span><span class="sxs-lookup"><span data-stu-id="82d81-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="82d81-110">לאחר שנעשה זאת, באפשרותך לוודא שלמשתמש יש זכויות מנהל לאתר OneDrive על-ידי ביצוע השלבים [להוספת admin עבור כונן onedrive המשתמש](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="82d81-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="82d81-111">לקבלת מידע נוסף אודות רמות הרשאה, עיין במאמר, [הכרת רמות הרשאה ב-SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="82d81-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
