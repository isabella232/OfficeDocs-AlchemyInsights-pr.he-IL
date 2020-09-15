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
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>פתרון בעיות גישה שנדחו על-ידי הודעות לאתרי OneDrive for Business

בעיה זו מתרחשת לעתים קרובות, כאשר משתמש נמחק ונוצר מחדש באמצעות אותו שם ראשי של המשתמש (UPN). החשבון החדש נוצר באמצעות ערך שונה של PUID (מזהה ייחודי של Passport). כאשר המשתמש מנסה לגשת לאוסף אתרים או לOneDrive שלו, למשתמש יש PUID שגוי. תרחיש נוסף כולל סינכרון מדריכי כתובות עם יחידה ארגונית של Active Directory (OU). אם המשתמשים כבר נכנסו ל-SharePoint ולאחר מכן מועברים ל-OU אחר ומסונכרנים מחדש ב-SharePoint, הם עשויים להיתקל בבעיה זו.

1. כדי לפתור בעיה זו, עליך לשחזר את ה-UPN המקורי בשלבים המפורטים במאמר, [לשחזר משתמש ב-Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. אם אין באפשרותך לשחזר את המשתמש המקורי, עליך להסיר את המשתמש הישן מאתר OneDrive באמצעות שלבים אלה, [להסיר משתמש מרשימת פרטי המשתמש](). 
3. לאחר ביצוע פעולה זו, באפשרותך לוודא שלמשתמש יש זכויות מנהל מערכת לאתר OneDrive על-ידי ביצוע השלבים [להוספת מנהל מערכת עבור OneDrive של משתמש](https://docs.microsoft.com/sharepoint/manage-user-profiles)

לקבלת מידע נוסף אודות רמות הרשאה, עיין במאמר [הכרת רמות הרשאה ב-SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
