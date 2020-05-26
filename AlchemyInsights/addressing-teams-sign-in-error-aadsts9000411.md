---
title: שגיאת כניסה לצוותים המיעון AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357880"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>שגיאת כניסה לצוותים המיעון AADSTS9000411

בעת הכניסה לצוותי Microsoft, ייתכן שתקבל את השגיאה: **מצטערים, אך יש לנו בעיה בחתימת החתימה שלך ב-AADSTS9000411: הבקשה אינה מעוצבת כראוי. הפרמטר "login_hint" משוכפל.**

כדי לטפל בבעיה זו, נא ודא שלקוחות צוותי Microsoft מתעדכנים. לקבלת מידע נוסף אודות עדכון הלקוח, ראה [עדכון צוותי Microsoft](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

אם אין באפשרותך לעדכן את הלקוח מסיבה כלשהי, התנתקות הלקוח תנקה את רוב הנתונים המאוחסנים במטמון. עם זאת, אם עדיין יש לך בעיות לאחר התנתקות/כניסה, צא מהקבוצות ובבקשה נקה את מטמון הלקוח על-ידי ביצוע הפעולות הבאות:
1. סגור את צוותי Microsoft.
2. עבור אל:%appdata%\ucet\mols\dute\n ומחק את כל הקבצים.
3. פתח מחדש את צוותי Microsoft.
