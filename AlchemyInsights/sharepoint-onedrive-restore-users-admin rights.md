---
title: פתרון בעיות של Access הודעות אל נדחתה OneDrive עבור אתרים עסקיים
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: b394cc1441187133d8829cfc5fb0c1edbd71fd96
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223425"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="da5e8-102">פתרון בעיות של Access הודעות אל נדחתה OneDrive עבור אתרים עסקיים</span><span class="sxs-lookup"><span data-stu-id="da5e8-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="da5e8-103">בעיה זו מתרחשת לעתים קרובות כאשר משתמש נמחקת ונוצרת מחדש עם אותו השם העיקרי של המשתמש (UPN).</span><span class="sxs-lookup"><span data-stu-id="da5e8-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="da5e8-104">החשבון החדש נוצר באמצעות ערך ה-PUID (מזהה ייחודי של Passport) שונה.</span><span class="sxs-lookup"><span data-stu-id="da5e8-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="da5e8-105">כאשר המשתמש מנסה לגשת לאוסף אתרים או OneDrive שלהם, יש למשתמש של ה-PUID שגוי.</span><span class="sxs-lookup"><span data-stu-id="da5e8-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="da5e8-106">תרחיש השני כרוך סינכרון ספריות עם יחידה ארגונית של Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="da5e8-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="da5e8-107">אם יש כבר נכנסו ל- SharePoint, ולאחר מכן הם הועברו לתפריט OU שונים ומשתמשים resynced עם SharePoint, עלול להיתקל בבעיה זו.</span><span class="sxs-lookup"><span data-stu-id="da5e8-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="da5e8-108">כדי לפתור בעיה זו אמורה לשחזר UPN המקורי עם השלבים במאמר,[שחזור משתמש ב- Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="da5e8-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="da5e8-109">לאחר מכן, באפשרותך לוודא שלמשתמש יש זכויות מנהל לאתר OneDrive על-ידי ביצוע השלבים הבאים כדי [admin הוספה עבור OneDrive של משתמש](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="da5e8-109">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="da5e8-110">לקבלת מידע נוסף אודות רמות הרשאה, עיין במאמר, [הכרת רמות הרשאה ב- SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="da5e8-110">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
