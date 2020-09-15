---
title: Active Directory אינו מסתנכרן
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697630"
---
# <a name="active-directory-not-syncing"></a>Active Directory אינו מסתנכרן

אם אתה מקבל שגיאות סינכרון, כגון "ללא סינכרון אחרון", או להבחין במצב סינכרון מדריכי כתובות בפורטל מנהל המערכת של Office, מופיעה ההודעה "סינכרון אחרון של יותר מ-3 ימים", ייתכן שAADConnect יש הגדרות שגויות או הרשאות לא מספיקות לביצוע סינכרון.  

התקנה מחדש של AADConnect באמצעות הגדרות אקספרס עשויה לפתור את הבעיה במהירות:

1. [הורד את הגירסה העדכנית ביותר של AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [בצע את ההוראות להתקנה מהירה](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

לקבלת מידע נוסף אודות חשבונות שירות של AADConnect, ראה [התחברות והרשאות בנושא תכלת לספירה: חשבונות והרשאות](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
