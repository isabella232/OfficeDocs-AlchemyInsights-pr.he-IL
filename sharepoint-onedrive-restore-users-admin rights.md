---
title: הענק למשתמשים גישה SharePoint ו- OneDrive
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
ms.openlocfilehash: ae4d2c00be6387744bdc84e1d8a021530f80f8fa
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/04/2019
ms.locfileid: "34715213"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="a9d02-102">הענק למשתמשים גישה SharePoint ו- OneDrive</span><span class="sxs-lookup"><span data-stu-id="a9d02-102">Give users access to SharePoint and OneDrive</span></span>

<p><span data-ttu-id="a9d02-103"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">בעיה זו מתרחשת לעתים קרובות כאשר משתמש נמחקת ונוצרת מחדש עם אותו השם העיקרי של המשתמש (UPN). החשבון החדש נוצר באמצעות ערך ה-PUID (מזהה ייחודי של Passport) שונה. כאשר המשתמש מנסה לגשת לאוסף אתרים או OneDrive שלהם, יש למשתמש של ה-PUID שגוי. תרחיש השני כרוך סינכרון ספריות עם יחידה ארגונית של Active Directory (OU). אם יש כבר נכנסו ל- SharePoint, ולאחר מכן הם הועברו לתפריט OU שונים ומשתמשים resynced עם SharePoint, עלול להיתקל בבעיה זו.</span></span><span class="sxs-lookup"><span data-stu-id="a9d02-103"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN). The new account is created by using a different PUID (Passport Unique ID) value. When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID. A second scenario involves directory synchronization with an Active Directory organizational unit (OU). If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span></span></p> <p><span data-ttu-id="a9d02-104"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">כדי לפתור בעיה זו אמורה לשחזר UPN המקורי עם השלבים במאמר, <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide">שחזור משתמש ב- Office 365.</a></span></span><span class="sxs-lookup"><span data-stu-id="a9d02-104"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">To resolve this issue you should restore the original UPN with the steps in the article, <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide">Restore a user in Office 365.</a></span></span></span></p> <p><span data-ttu-id="a9d02-105"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">לאחר מכן, באפשרותך לוודא שלמשתמש יש זכויות מנהל לאתר OneDrive על-ידי ביצוע השלבים הבאים כדי <a href="https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive">להוסיף של הניהול עבור OneDrive המשתמש.</a></span></span><span class="sxs-lookup"><span data-stu-id="a9d02-105"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to <a href="https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive">Add admin's for a user's OneDrive.</a></span></span></span></p> <p><span data-ttu-id="a9d02-106"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">לקבלת מידע נוסף אודות רמות הרשאה, עיין במאמר, <a href="https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels">הכרת רמות הרשאה ב- SharePoint.</a>&nbsp;</span></span><span class="sxs-lookup"><span data-stu-id="a9d02-106"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">For more information on permission levels, see the article, <a href="https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels">Understanding permission levels in SharePoint.</a>&nbsp;</span></span></span></p>
