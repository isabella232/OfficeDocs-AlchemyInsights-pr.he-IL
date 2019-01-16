---
title: 646 כיצד להגדיר AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: e4ba295cd0661c3454180dd6a15895123840389e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28291930"
---
# <a name="configure-sync-features"></a>קביעת תצורה של תכונות סינכרון

התחבר AD תכלת הרקיע כולל מספר תכונות אשר מופעלות כברירת מחדל, או שבאפשרותך להפוך לזמינות במועד מאוחר יותר. תכונות מסוימות דורשות קביעת תצורה נוספת בסביבות מסוימות.
  
- מגבלות [סינון](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) האובייקטים יסונכרנו AD תכלת הרקיע. כברירת מחדל, כל המשתמשים, אנשי קשר, קבוצות, Windows 10 חשבונות מחשב מסונכרנים. באפשרותך לכלול או לא לכלול אובייקטים לפי תחומים, יחידות ארגוניות או תכונות אחרות. 
    
- [Syncronization ה-hash של סיסמת](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) מסנכרן hash סיסמה מ- Active Directory מקומי כדי AD תכלת הרקיע. פעולה זו מאפשרת ניהול סיסמאות במיקום אחד, אך שימוש בסיסמה זהה בשני המקומית סביבות ענן. מכיוון שמקור סמכותי Active Directory, באפשרותך להשתמש מדיניות סיסמה משלך. 
    
- [איפוס סיסמה בשירות עצמי (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) מאפשר למשתמשים לאפס את הסיסמאות שלהם בענן בעת החלת מדיניות הסיסמה המקומית שלך עדיין. 
    
- [Writeback התקן](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) מאפשר ההתקנים הרשומים ב- AD תכלת הרקיע להיכתב בחזרה ל- Active Directory מקומי כך הם יכולים לשמש לקבלת גישה מותנית. 
    
- [בטעות מנע מחיקות](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) מופעלת כברירת מחדל כדי לסייע למנוע מחיקות האובייקט בו-זמנית יותר מדי (יותר מ- 500 אובייקטים לפי סינכרון). באפשרותך לשנות הגדרה זו כדי לענות על הצרכים של הארגון שלך. 
    
- [שדרוג אוטומטי](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) מופעלת כברירת מחדל עבור התקנות מפורשת ו מסייע להבטיח שהגירסה של התחברות AD תכלת הרקיע הוא תמיד הנוכחי. 
    

