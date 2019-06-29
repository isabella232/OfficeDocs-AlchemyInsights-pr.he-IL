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
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 42a56b17e41649d979cf442909e8357eb262cf9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35354798"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>פתרון בעיות של Access הודעות אל נדחתה OneDrive עבור אתרים עסקיים

בעיה זו מתרחשת לעתים קרובות כאשר משתמש נמחקת ונוצרת מחדש עם אותו השם העיקרי של המשתמש (UPN). החשבון החדש נוצר באמצעות ערך ה-PUID (מזהה ייחודי של Passport) שונה. כאשר המשתמש מנסה לגשת לאוסף אתרים או OneDrive שלהם, יש למשתמש של ה-PUID שגוי. תרחיש השני כרוך סינכרון ספריות עם יחידה ארגונית של Active Directory (OU). אם יש כבר נכנסו ל- SharePoint, ולאחר מכן הם הועברו לתפריט OU שונים ומשתמשים resynced עם SharePoint, עלול להיתקל בבעיה זו.

כדי לפתור בעיה זו אמורה לשחזר UPN המקורי עם השלבים במאמר,[שחזור משתמש ב- Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

לאחר מכן, באפשרותך לוודא שלמשתמש יש זכויות מנהל לאתר OneDrive על-ידי ביצוע השלבים הבאים כדי [admin הוספה עבור OneDrive של משתמש](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

לקבלת מידע נוסף אודות רמות הרשאה, עיין במאמר, [הכרת רמות הרשאה ב- SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
