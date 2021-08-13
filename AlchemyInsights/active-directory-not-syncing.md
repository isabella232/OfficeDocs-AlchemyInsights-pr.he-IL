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
ms.openlocfilehash: 4bfbe6b2dd9a2112f0cb7af0d6e7a46693bc70680895fd674ddb0332b7071797
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53937102"
---
# <a name="active-directory-not-syncing"></a>Active Directory אינו מסתנכרן

אם אתה מקבל שגיאות סינכרון, כגון "ללא סינכרון לאחרונה", או שים לב למצב סינכרון מדריכי הכתובות בפורטל הניהול של Office רשום "הסינכרון האחרון לפני יותר מ- 3 ימים", ייתכן של- AADConnect יש הגדרות שגויות או הרשאות לא מספיקות לביצוע סינכרון.  

התקנה מחדש של AADConnect באמצעות הגדרות מהירות עשויה לפתור את הבעיה במהירות:

1. [הורד את הגירסה העדכנית ביותר של AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [בצע את ההוראות להתקנה מהירה.](/azure/active-directory/hybrid/how-to-connect-install-express)

Azure AD Connect חייב להיות מותקן ב- Windows Server 2012 או גירסה מאוחרת יותר. שרת זה חייב להיות מצורף לתחום והוא יכול להיות בקר תחום או שרת עמית. לקבלת רשימה מלאה של דרישות התחברות של Azure AD ודרישות מוקדמות, עיין בדרישות מוקדמות עבור [Azure AD התחברות.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

לקבלת מידע נוסף אודות חשבונות שירות של AADConnect, ראה [Azure AD התחברות: חשבונות והרשאות](/azure/active-directory/hybrid/reference-connect-accounts-permissions).
