---
title: 646 כיצד להגדיר את AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704490"
---
# <a name="configure-sync-features"></a>קביעת תצורה של תכונות סינכרון

חיבור תכלת לספירה כולל כמה תכונות הזמינות כברירת מחדל, או שניתן להפוך אותן לזמינות במועד מאוחר יותר. תכונות מסוימות דורשות תצורה נוספת בסביבות ספציפיות.

- מגבלות [סינון](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) האובייקטים מסונכרנים עם התכלת לספירה. כברירת מחדל, כל המשתמשים, אנשי הקשר, הקבוצות ו-Windows 10 חשבונות מחשב מסונכרנים. באפשרותך לכלול או לא לכלול אובייקטים בהתבסס על תחומים, רכיבי Ou או תכונות אחרות.

- [סינכרון hash של סיסמאות](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) מסנכרן את קוד ה-hash של הסיסמה ממדריך הכתובות המקומי של Active Directory לכיוון תכלת לספירה. פעולה זו מאפשרת ניהול סיסמאות במיקום אחד, אך שימוש באותה סיסמה בסביבות מקומיות ובסביבת ענן. מכיוון ש-Active Directory הוא המקור הסמכותי, באפשרותך להשתמש במדיניות הסיסמה שלך.

- [איפוס סיסמה בשירות עצמי (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) מאפשר למשתמשים לאפס את הסיסמאות שלהם בענן בזמן שהם עדיין מיישמים את מדיניות הסיסמה המקומית שלך.

- [התקן writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) מאפשר התקנים רשומים בתכלת AD להיכתב בחזרה אל active Directory המקומי כדי שניתן יהיה להשתמש בהם לקבלת גישה מותנית.

- [מניעת מחיקה בשוגג](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) מופעלת כברירת מחדל כדי לסייע במניעת מחיקות של אובייקטים בו רבים מדי (יותר מ-500 אובייקטים לכל סינכרון). באפשרותך לשנות הגדרה זו כדי לענות על הצרכים של הארגון שלך.

- [שדרוג אוטומטי](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) מופעל כברירת מחדל עבור התקנות מפורשות ומסייע להבטיח שגירסת החיבור של ' תכלת לספירה ' תהיה תמיד עדכנית.
