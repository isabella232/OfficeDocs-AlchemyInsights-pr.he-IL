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
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826380"
---
# <a name="teams-admin-center"></a>מרכז הניהול של Teams

קבל מידע נוסף על ניהול Teams באמצעות [מרכז הניהול של Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

אם אינך מצליח לגשת למרכז הניהול של Teams, בדוק את הפריטים הבאים:

- ודא שאפשרת את [כתובות ה- IP וכתובות ה- URL המתאימות ב- Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) של כל ההתקנים ההיקפיים (חומת אש וכו‘) או בחוקי חומת האש במחשב המקומי שלך.
- ודא שההתחברות שבה אתה משתמש כדי לגשת לפורטל הניהול של Teams מתאימה לשם המשתמש שלך המופיע ב-[פורטל הניהול של Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

אם המשתמשים אינם מופיעים במרכז הניהול של Teams, בדוק:

- האם יצרת משתמשים או רשיונות שהוקצו ב- 24 השעות האחרונות? המתן לפחות 24 שעות לפני פתיחת כרטיס תמיכה.
- ודא שהקצית רשיונות מתאימים?
- אם יש לך Active Directory מקומי, ודא שהערך [של msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) או כתובת SIP בשדה ProxyAddresses ב- Active Directory המקומי שלך הוא ייחודי והתבנית תואמת ללגימה:**שם** המשתמש של המשתמש ממרכז הניהול של [Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- אם בכוונתך לשמור פריסה של Skype for Business Server ולהגדיר משתמשים ביתיים באופן מקומי ומקוון: פעל בהתאם ל"הגדרת היברידיות עם **Teams ו- Skype for Business Online"** בלוח הבקרה של Skype for Business Server והעביר משתמשים למצב מקוון.
