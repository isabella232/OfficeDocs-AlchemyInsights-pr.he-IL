---
title: 'AIP: מדיניות שאינה מתנהגת כמצופה'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 527556fcb02525eb88ea992c38a2ddfcba6f9453
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506559"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: מדיניות שאינה מתנהגת כמצופה

הגנת מידע תכלת: מדיניות שאינה מתנהגת כמצופה, עיין בהוראות הבאות לקבלת הנחיות מומלצות לסוגיות מדיניות שונות:

1. אם נתקלת בבעיות בסימונים חזותיים, עיין [במועד ההחלה של סימונים חזותיים](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. אם אתה נתקל בבעיות עם תיוג אוטומטי, עיין [באופן ההגדרה של תנאים לסיווג אוטומטי ומומלץ עבור הגנת מידע תכלת](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) [ואילו סוגי המידע הרגישים](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)מחפשים.
3. אם נתקלת בבעיות בהגנה על מקורי/Pfile, עיין [בתצורת ה-API של הקובץ](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. בדוק אם אתה משתמש במדיניות מתוחם שאינה [מוגדרת כראוי: כיצד לקבוע את תצורת המדיניות ' הגנה מפני מידע ' עבור משתמשים ספציפיים באמצעות מדיניות מתוחם](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. אם תיוג אוטומטי אינו פועל עבור Outlook בעת צירוף מסמך המסומן בתווית, ודא שהמאפיין DRMEncryptProperty אינו מוגדר כמתואר כאן: [הגדרות הרישום של IRM עבור אבטחה](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

אם עדיין נתקלת בבעיות, נא לאסוף את יומני הלקוחות של הגנת המידע התכלת ולצרף את היומנים המיוצאים לכרטיס זה.

1. פתח מסמך של Office או צור מייל חדש ב-Outlook.
2. לחץ **Protect/Sensitivity**על  >  **עזרה ומשוב של הגנה**/רגישות.
3. לחץ על **ייצוא יומני רישום**.
4. שמור את יומני הרישום בבחירת המיקום שלך וצרף אותם לבקשת שירות זו.

משאבים נוספים:

- [כיצד להגדיר תווית עבור סימונים חזותיים עבור הגנת מידע תכלת](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [סקירת התיעוד של הגנת מידע תכלת](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [שימוש בתוויות רגישות ביישומי Office](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

