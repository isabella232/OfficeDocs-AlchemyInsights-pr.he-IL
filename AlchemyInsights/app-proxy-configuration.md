---
title: תצורת Proxy של יישום
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7800"
ms.openlocfilehash: 835bfc59f77b31dc9a37c98db911505e2c7a758b37406dfc4da2d139afa61db5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951566"
---
# <a name="app-proxy-configuration"></a>תצורת Proxy של יישום

1. כדי להבין כיצד להגדיר יישום Proxy של יישום בתוך Azure AD כדי לחשוף את היישומים המקומיים שלך לענן, ראה כיצד להגדיר [יישום Proxy של יישום](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).
2. כניסה יחידה (SSO) מאפשרת למשתמשים שלך לגשת ליישום מבלי לאימות מספר פעמים. היא מאפשרת לאימות היחיד להתרחש בענן, מול Azure Active Directory ומאפשרת לשירות או למחבר להתחזות למשתמש כדי להשלים את אתגרי האימות הנוספות של היישום. כדי ללמוד עוד, ראה [כיצד להגדיר כניסה יחידה ליישום Proxy של יישום](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).
3. השתמש [במאמר זה כדי](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) לפתור בעיות נפוצות שאנשים יתמודדו מולן בעת יצירת יישום Proxy חדש של יישום.
4. אם אתה נתקל בבעיה בהגדרת אימות מסולסל ליישום שלך, ייתכן שתצטרך לפתור בעיות של תצורות הקצאה מאולצות של [Kerberos](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) עבור Proxy של יישום או פעל בהתאם להנחיות לקביעת התצורה של היישום [עם PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) כדי לפתור את הבעיה.
