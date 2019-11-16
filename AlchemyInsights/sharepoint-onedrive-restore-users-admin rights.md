---
title: פתרון בעיות ב-Access דחה הודעות ל-OneDrive עבור אתרים עסקיים
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 3c40ad76a8961a3d0b4963483291c2a1364c51d3
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 11/15/2019
ms.locfileid: "37766712"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>פתרון בעיות ב-Access דחה הודעות ל-OneDrive עבור אתרים עסקיים

בעיה זו מתרחשת לעתים קרובות כאשר משתמש נמחק ונוצר מחדש עם אותו שם ראשי של משתמש (UPN). החשבון החדש נוצר על-ידי שימוש בערך PUID (מזהה Passport ייחודי) אחר. כשהמשתמש מנסה לגשת לאוסף אתרים או ל-OneDrive שלהם, למשתמש יש PUID שגוי. תרחיש שני כולל סינכרון ספריות עם יחידה ארגונית של Active Directory (OU). אם משתמשים כבר החתימו ב-SharePoint ולאחר מכן מועברים ל-OU אחר ומסונכרנים מחדש עם SharePoint, הם עלולים להיתקל בבעיה זו.

1. כדי לפתור בעיה זו, עליך לשחזר את ה-UPN המקורי עם השלבים במאמר, [לשחזר משתמש ב-Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. אם אין באפשרותך לשחזר את המשתמש המקורי, עליך להסיר את המשתמש הישן מהאתר OneDrive באמצעות שלבים אלה, [להסיר משתמש מרשימת פרטי המשתמש](). 
3. לאחר שנעשה זאת, באפשרותך לוודא שלמשתמש יש זכויות מנהל לאתר OneDrive על-ידי ביצוע השלבים [להוספת admin עבור כונן onedrive המשתמש](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

לקבלת מידע נוסף אודות רמות הרשאה, עיין במאמר, [הכרת רמות הרשאה ב-SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
