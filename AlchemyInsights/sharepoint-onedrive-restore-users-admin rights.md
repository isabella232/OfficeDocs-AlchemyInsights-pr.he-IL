---
title: פתרון בעיות של Access הודעות אל נדחתה OneDrive עבור אתרים עסקיים
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: d47ce80bdd07a25d9724057edf0289808a00a3db
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232527"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>פתרון בעיות של Access הודעות אל נדחתה OneDrive עבור אתרים עסקיים

בעיה זו מתרחשת לעתים קרובות כאשר משתמש נמחקת ונוצרת מחדש עם אותו השם העיקרי של המשתמש (UPN). החשבון החדש נוצר באמצעות ערך ה-PUID (מזהה ייחודי של Passport) שונה. כאשר המשתמש מנסה לגשת לאוסף אתרים או OneDrive שלהם, יש למשתמש של ה-PUID שגוי. תרחיש השני כרוך סינכרון ספריות עם יחידה ארגונית של Active Directory (OU). אם יש כבר נכנסו ל- SharePoint, ולאחר מכן הם הועברו לתפריט OU שונים ומשתמשים resynced עם SharePoint, עלול להיתקל בבעיה זו.

1. כדי לפתור בעיה זו אמורה לשחזר UPN המקורי עם השלבים במאמר,[שחזור משתמש ב- Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. אם אין אפשרות לשחזר את המשתמש המקורי יש להסיר את המשתמש הישן מאתר OneDrive באמצעות השלבים הבאים, [להסיר משתמש מהרשימה פרטי המשתמש](). 
3. לאחר מכן, באפשרותך לוודא שלמשתמש יש זכויות מנהל לאתר OneDrive על-ידי ביצוע השלבים הבאים כדי [admin הוספה עבור OneDrive של משתמש](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

לקבלת מידע נוסף אודות רמות הרשאה, עיין במאמר, [הכרת רמות הרשאה ב- SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
