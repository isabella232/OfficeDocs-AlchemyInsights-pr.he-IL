---
title: מרכז הניהול של Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670365"
---
# <a name="teams-admin-center"></a>מרכז הניהול של Teams

קבל מידע נוסף על ניהול Teams באמצעות [מרכז הניהול של Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

אם אינך מצליח לגשת למרכז הניהול של Teams, בדוק את הפריטים הבאים:

- ודא שאפשרת את [כתובות ה- IP וכתובות ה- URL המתאימות ב- Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) של כל ההתקנים ההיקפיים (חומת אש וכו‘) או בחוקי חומת האש במחשב המקומי שלך.
- ודא שההתחברות שבה אתה משתמש כדי לגשת לפורטל הניהול של Teams מתאימה לשם המשתמש שלך המופיע ב-[פורטל הניהול של Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

אם המשתמשים אינם מופיעים במרכז הניהול של Teams, בדוק:

- האם יצרת משתמשים או רשיונות שהוקצו ב- 24 השעות האחרונות? המתן לפחות 24 שעות לפני פתיחת כרטיס תמיכה.
- ודא שהקצית רשיונות מתאימים?
- אם יש לך מדריך Active Directory מקומי, ודא [שהערך של msRTCSIP-PrimaryUserAddress או כתובת SIP בשדה ProxyAddresses ב-Active Directory המקומי שלך הוא ייחודי והתבנית תואמת](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) Sip:**Username** של המשתמש [ממרכז הניהול של Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- אם בכוונתך לשמור על הפריסה של Skype for Business Server ולהגדיר משתמשים באופן מקומי ומקוון: עקוב אחר **ההגדרה ' הכלאה משולבת עם teams ו-Skype For Business online** ' בלוח הבקרה של Skype For business Server והעברת משתמשים באופן מקוון.
