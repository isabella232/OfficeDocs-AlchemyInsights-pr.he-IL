---
title: Active Directory אינו מסתנכרן
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: d4615d335b9aeef69148cd93ff9f44bec6d7d876
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314205"
---
# <a name="active-directory-not-syncing"></a>Active Directory אינו מסתנכרן

אם אתה מקבל שגיאות סינכרון, כגון "ללא סינכרון לאחרונה", או שים לב למצב סינכרון מדריכי הכתובות בפורטל הניהול של Office רשום "Last synced לפני יותר מ- 3 ימים", ייתכן של- AADConnect יש הגדרות שגויות או הרשאות לא מספיקות לביצוע סינכרון.  

התקנה מחדש של AADConnect באמצעות הגדרות מהירות עשויה לפתור את הבעיה במהירות:

1. [הורד את הגירסה העדכנית ביותר של AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [בצע את ההוראות להתקנה מהירה.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

Azure AD Connect חייב להיות מותקן ב- Windows Server 2012 או גירסה מאוחרת יותר. שרת זה חייב להיות מצורף לתחום והוא יכול להיות בקר תחום או שרת עמית. לקבלת רשימה מלאה של דרישות התחברות של Azure AD ודרישות מוקדמות, עיין בדרישות [מוקדמות](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)עבור Azure AD התחברות .

לקבלת מידע נוסף אודות חשבונות שירות AADConnect, ראה [Azure AD התחברות: חשבונות והרשאות](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
