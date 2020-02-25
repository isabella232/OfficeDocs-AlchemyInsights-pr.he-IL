---
title: Active Directory אינו מסנכרן
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265197"
---
# <a name="active-directory-not-syncing"></a>Active Directory אינו מסנכרן

אם אתה מקבל שגיאות סינכרון, כגון "ללא סנכרון עדכני", או שים לב שמצב סינכרון הספריות בפורטל הניהול של Office אומר: "הסינכרון האחרון לפני יותר מ-3 ימים", יתכן כי AADConnect יש הגדרות שגויות או לא מספיקות הרשאות לביצוע סינכרון.  

התקנה מחדש של AADConnect באמצעות הגדרות מהירות עשויה לפתור את הבעיה במהירות:

1. [הורד את הגירסה העדכנית ביותר של AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [בצע את ההוראות עבור התקנה מפורשת](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

לקבלת מידע נוסף על AADConnect חשבונות שירות, ראה [תכלת התחברות: חשבונות והרשאות](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
