---
title: מרכז הניהול של Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 29e54e0f8255b4ce84c433f2cc827aaedf35327626f0095788faef802763bc53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049345"
---
# <a name="teams-admin-center"></a>מרכז הניהול של Teams

קבל מידע נוסף על ניהול Teams באמצעות [מרכז הניהול של Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

אם אינך מצליח לגשת למרכז הניהול של Teams, בדוק את הפריטים הבאים:

- ודא שאפשרת את [כתובות ה- IP וכתובות ה- URL המתאימות ב- Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) של כל ההתקנים ההיקפיים (חומת אש וכו‘) או בחוקי חומת האש במחשב המקומי שלך.
- ודא שההתחברות שבה אתה משתמש כדי לגשת לפורטל הניהול של Teams מתאימה לשם המשתמש שלך המופיע ב-[פורטל הניהול של Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

אם המשתמשים אינם מופיעים במרכז הניהול של Teams, בדוק:

- האם יצרת משתמשים או רשיונות שהוקצו ב- 24 השעות האחרונות? המתן לפחות 24 שעות לפני פתיחת כרטיס תמיכה.
- ודא שהקצית רשיונות מתאימים?
- אם יש לך Active Directory מקומי, ודא שהערך [של msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) או כתובת SIP בשדה ProxyAddresses ב- Active Directory המקומי שלך הוא ייחודי והתבנית תואמת ללגימה:**שם** המשתמש של המשתמש [מתוך מרכז הניהול של Microsoft 365.](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)
- אם בכוונתך לשמור פריסה של Skype for Business Server ומשתמשים יש להם משתמשים מקומיים ומקוון: בצע את "הגדרת היברידית **עם Teams ו- Skype for Business Online"** בלוח הבקרה של Skype for Business Server ולהעביר משתמשים באופן מקוון.
