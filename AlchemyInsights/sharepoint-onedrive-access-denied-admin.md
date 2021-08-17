---
title: פתרון בעיות Access הודעות שנדחתה
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9acde72f82a27c9f2faa2cf4d0417374aa5a294234da96080dc0498d07639248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085229"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>פתרון Access הודעות שנדחתה ב- Sharepoint/OneDrive הניהול של Sharepoint

אם אתה מקבל הודעה שנדחתה על-ידי גישה בעת ניסיון לנווט אל מרכז הניהול של Sharepoint/OneDrive, הקפד להקצות [רשיון למשתמש](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). אם למשתמש יש רשיון, עליך גם לוודא שהוקצה לו תפקיד [מנהל מערכת](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) שיש לו אפשרות לגשת למרכזי הניהול.

בעיה זו עשויה להתרחש גם כאשר משתמש נמחק וניווצר מחדש עם אותו שם ראשי של משתמש (UPN). החשבון החדש נוצר באמצעות ערך PUID אחר (מזהה ייחודי של Passport). כאשר המשתמש מנסה לגשת לאוסף אתרים או OneDrive, למשתמש יש מזהה PU שגוי. תרחיש שני כרוך בסינכרון מדריכי כתובות עם יחידה ארגונית של Active Directory (OU). אם המשתמשים כבר מחוברים ל- SharePoint, ולאחר מכן מועברים ל- OU אחר ומסונכרןים מחדש עם SharePoint, הם עשויים להיתקל בבעיה זו.

כדי לפתור בעיה זו, עליך לשחזר את UPN המקורי עם השלבים במאמר, [שחזר משתמש ב- Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

הערה: אם מרכז OneDrive או SharePoint מנהל מערכת אינו זמין למשתמשים מרובים שהיו להם גישה בעבר, ייתכן שיש בעיית שירות זמנית.  [בדוק את לוח המחוונים של תקינות השירות](https://portal.office.com/adminportal/home#/servicehealth).


