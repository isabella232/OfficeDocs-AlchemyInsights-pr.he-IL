---
title: פתרון Access הודעות שנדחתה לאתרי OneDrive for Business שלך
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
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957794"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>פתרון Access הודעות שנדחתה לאתרי OneDrive for Business שלך

בעיה זו מתרחשת לעתים קרובות כאשר משתמש נמחק וניווצר מחדש עם אותו שם ראשי של משתמש (UPN). החשבון החדש נוצר באמצעות ערך PUID אחר (מזהה ייחודי של Passport). כאשר המשתמש מנסה לגשת לאוסף אתרים או OneDrive, למשתמש יש מזהה PU שגוי. תרחיש שני כרוך בסינכרון מדריכי כתובות עם יחידה ארגונית של Active Directory (OU). אם המשתמשים כבר מחוברים ל- SharePoint, ולאחר מכן מועברים ל- OU אחר ומסונכרןים מחדש עם SharePoint, הם עשויים להיתקל בבעיה זו.

1. כדי לפתור בעיה זו, עליך לשחזר את UPN המקורי עם השלבים במאמר, [שחזר משתמש ב- Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)
2. אם אין באפשרותך לשחזר את המשתמש המקורי, עליך להסיר את המשתמש הישן מהאתר OneDrive באמצעות שלבים אלה, [הסר משתמש מרשימת פרטי המשתמש](). 
3. לאחר הליך זה, באפשרותך לוודא שלמשתמש יש זכויות מנהל מערכת באתר [](https://docs.microsoft.com/sharepoint/manage-user-profiles) OneDrive על-ידי ביצוע השלבים להוספת מנהל מערכת עבור OneDrive

לקבלת מידע נוסף אודות רמות הרשאה, עיין במאמר הכרת [רמות הרשאה ב- SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
