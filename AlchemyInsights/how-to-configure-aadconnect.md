---
title: 646 כיצד לקבוע את התצורה של AADConnect
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
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963644"
---
# <a name="configure-sync-features"></a>קביעת תצורה של תכונות סינכרון

Azure AD התחברות כוללת כמה תכונות זמינות כברירת מחדל, או שזמינה במועד מאוחר יותר. תכונות מסוימות דורשות קביעת תצורה נוספת בסביבות ספציפיות.

- [סינון מגביל](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) את האובייקטים מסונכרנים עם Azure AD. כברירת מחדל, כל המשתמשים, אנשי הקשר, הקבוצות וחשבונות Windows 10 מסונכרנים. באפשרותך לכלול או לא לכלול אובייקטים בהתבסס על תחומים, יחידות OUs או תכונות אחרות.

- [סינכרון Hash של](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) סיסמה מסנכרן את קוד ה- Hash של הסיסמה מ- Active Directory המקומי ל- Azure AD. פעולה זו מאפשרת ניהול סיסמאות במיקום אחד, אך שימוש באותה סיסמה הן בסביבות מקומיות ובענן. מאחר ש- Active Directory הוא המקור הסמכותי, באפשרותך להשתמש במדיניות הסיסמה שלך.

- [איפוס סיסמה בשירות עצמי (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) מאפשר למשתמשים לאפס את הסיסמאות שלהם בענן תוך החלת מדיניות הסיסמה המקומית שלך.

- [כתיבה חוזרת](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) של מכשיר מאפשרת לכתוב מכשירים רשומים ב- Azure AD בחזרה ל- Active Directory המקומי, כדי שתוכל להשתמש בהם לגישה מותית.

- [מניעת מחיקות בשוגג](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) זמינה כברירת מחדל כדי לסייע במניעת מחיקות אובייקטים בו-זמניות רבות מדי (יותר מ- 500 אובייקטים לכל סינכרון). באפשרותך לשנות הגדרה זו כך שתתן את צרכי הארגון שלך.

- [שדרוג אוטומטי](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) זמין כברירת מחדל עבור התקנות מפורשות ומבטיח שהגירסה של Azure AD התחברות תמיד עדכנית.
