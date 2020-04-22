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
ms.openlocfilehash: a83936acf969926c113b28ceb22b006cdb96e2b4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692802"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>פתרון בעיות ב-Access דחה הודעות ל-OneDrive עבור אתרים עסקיים

בעיה זו מתרחשת לעתים קרובות כאשר משתמש נמחק ונוצר מחדש עם אותו שם ראשי של משתמש (UPN). החשבון החדש נוצר על-ידי שימוש בערך PUID (מזהה Passport ייחודי) אחר. כשהמשתמש מנסה לגשת לאוסף אתרים או ל-OneDrive שלהם, למשתמש יש PUID שגוי. תרחיש שני כולל סינכרון ספריות עם יחידה ארגונית של Active Directory (OU). אם משתמשים כבר החתימו ב-SharePoint ולאחר מכן מועברים ל-OU אחר ומסונכרנים מחדש עם SharePoint, הם עלולים להיתקל בבעיה זו.

1. כדי לפתור בעיה זו עליך לשחזר את ה-UPN המקורי עם השלבים במאמר, [לשחזר משתמש ב-Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).
2. אם אין באפשרותך לשחזר את המשתמש המקורי, עליך להסיר את המשתמש הישן מהאתר OneDrive באמצעות שלבים אלה, [להסיר משתמש מרשימת פרטי המשתמש](). 
3. לאחר שנעשה זאת, באפשרותך לוודא שלמשתמש יש זכויות מנהל לאתר OneDrive על-ידי ביצוע השלבים [להוספת admin עבור כונן onedrive המשתמש](https://docs.microsoft.com/sharepoint/manage-user-profiles)

לקבלת מידע נוסף אודות רמות הרשאה, עיין במאמר, [הכרת רמות הרשאה ב-SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
