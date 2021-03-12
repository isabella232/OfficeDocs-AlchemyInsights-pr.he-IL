---
title: פתרון בעיות בהודעות של Access שנדחו
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707955"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>פתרון בעיות בהודעות של Access שנדחו במרכז הניהול של Sharepoint/OneDrive

אם אתה מקבל הודעת גישה שנדחתה בעת ניסיון לנווט למרכז הניהול של Sharepoint/OneDrive, ודא שאתה [מקצה רשיון למשתמש](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). אם למשתמש יש רשיון, עליך גם לוודא שהוא [מוקצה לתפקיד מנהל מערכת](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) שיכול לגשת למרכזי הניהול.

בעיה זו עלולה להתרחש גם כאשר משתמש נמחק ונוצר מחדש עם אותו שם ראשי של המשתמש (UPN). החשבון החדש נוצר באמצעות ערך שונה של PUID (מזהה ייחודי של Passport). כאשר המשתמש מנסה לגשת לאוסף אתרים או לOneDrive שלו, למשתמש יש PUID שגוי. תרחיש נוסף כולל סינכרון מדריכי כתובות עם יחידה ארגונית של Active Directory (OU). אם המשתמשים כבר נכנסו ל-SharePoint ולאחר מכן מועברים ל-OU אחר ומסונכרנים מחדש ב-SharePoint, הם עשויים להיתקל בבעיה זו.

כדי לפתור בעיה זו, עליך לשחזר את ה-UPN המקורי בשלבים המפורטים במאמר, [לשחזר משתמש ב-Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

הערה: אם מרכז הניהול של OneDrive או SharePoint אינו זמין למשתמשים מרובים שהיו ברשותם גישה בעבר, ייתכן שקיימת בעיה של שירות זמני.  [בדוק את לוח המחוונים של תקינות השירות](https://portal.office.com/adminportal/home#/servicehealth).


