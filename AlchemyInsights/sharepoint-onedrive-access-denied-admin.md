---
title: פתרון בעיות בהודעות שנדחו על-ידי Access
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 57919e6dbd81a5bf3b17fb067485e8eec23b7d4c
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051426"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>פתרון בעיות של הודעות שנדחו ב-Access במרכז ניהול Sharepoint/OneDrive

אם אתה מקבל הודעת גישה שנדחתה בעת ניסיון לגלוש אל מרכז ניהול Sharepoint/OneDrive, נא ודא שאתה [מקצה רשיון למשתמש](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). אם למשתמש יש רשיון, עליך גם לוודא [שהוקצו לו תפקיד מנהל](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) שיכול לגשת למרכזי הניהול.

בעיה זו עשויה להתרחש גם כאשר משתמש נמחק ונוצר מחדש עם אותו שם ראשי של משתמש (UPN). החשבון החדש נוצר על-ידי שימוש בערך PUID (מזהה Passport ייחודי) אחר. כשהמשתמש מנסה לגשת לאוסף אתרים או ל-OneDrive שלהם, למשתמש יש PUID שגוי. תרחיש שני כולל סינכרון ספריות עם יחידה ארגונית של Active Directory (OU). אם משתמשים כבר החתימו ב-SharePoint ולאחר מכן מועברים ל-OU אחר ומסונכרנים מחדש עם SharePoint, הם עלולים להיתקל בבעיה זו.

כדי לפתור בעיה זו, עליך לשחזר את ה-UPN המקורי עם השלבים במאמר, [לשחזר משתמש ב-Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

הערה: אם מרכז OneDrive או SharePoint Admin אינו זמין למשתמשים מרובים שהיו בעבר גישה, ייתכן שקיימת בעיית שירות זמנית.  [בדוק את לוח המחוונים של תקינות השירות](https://portal.office.com/adminportal/home#/servicehealth).


