---
title: 646 כיצד להגדיר את התצורה של AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722543"
---
# <a name="configure-sync-features"></a>קביעת תצורה של תכונות סינכרון

תכלת ההתחברות כוללת מספר תכונות הזמינות כברירת מחדל, או שניתן להפוך אותן לזמינות מאוחר יותר. תכונות מסוימות דורשות תצורה נוספת בסביבות ספציפיות.

- [סינון](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) מגביל את האובייקטים שהאובייקטים מסונכרנים לתכלת AD. כברירת מחדל, כל המשתמשים, אנשי הקשר, הקבוצות וחשבונות המחשבים של Windows 10 מסונכרנים. באפשרותך לכלול או לא לכלול אובייקטים המבוססים על קבוצות מחשבים, OUs או תכונות אחרות.

- [סינכרון hash של סיסמה](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) מסנכרן את קוד ה-hash של הסיסמה מהספריה הפעילה המקומית אל תכלת AD. פעולה זו מאפשרת ניהול סיסמאות במיקום אחד, אך שימוש באותה סיסמה הן בסביבות מקומיות והן בסביבת ענן. מכיוון ש-Active Directory הוא המקור הסמכותי, באפשרותך להשתמש במדיניות סיסמה משלך.

- [איפוס סיסמה של שירות עצמי (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) מאפשר למשתמשים לאפס את הסיסמאות שלהם בענן הצמתים תוך שהם עדיין מיישמים את מדיניות הסיסמה המקומית.

- כותב [המכשיר](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) מאפשר התקנים רשומים בתכלת AD כדי להיכתב חזרה ל-active Directory המקומי כדי שניתן יהיה להשתמש בהם עבור גישה מותנית.

- [מנע מחיקות בשוגג](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) כברירת מחדל כדי לסייע במניעת מחיקות של אובייקטים בו (יותר מ-500 אובייקטים לכל סינכרון). באפשרותך לשנות הגדרה זו כדי לענות על צרכי הארגון שלך.

- [שדרוג אוטומטי](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) מאופשר כברירת מחדל עבור התקנות מפורשת ומסייע להבטיח שגירסת ה-"כחול החיבור" שלך תהיה תמיד עדכנית.
