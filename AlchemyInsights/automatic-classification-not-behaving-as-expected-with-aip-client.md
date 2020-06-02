---
title: הסיווג האוטומטי אינו מתנהג כמצופה באמצעות לקוח AIP
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
- "4373"
ms.openlocfilehash: 22eeb6ba32e4e943efa2495a477ff394f3c135db
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: he-IL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508377"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>הסיווג האוטומטי אינו מתנהג כמצופה באמצעות לקוח AIP

הסיווג האוטומטי אינו מתנהג כמצופה, השתמש בהנחיות המומלצות הבאות:

1. אם נתקלת בבעיות בתיוג אוטומטי, ראה [כיצד להגדיר תנאים לסיווג אוטומטי ומומלץ עבור הגנת מידע תכלת](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) [ואילו סוגי המידע הרגישים](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)מחפשים.
2. בדוק אם אתה משתמש במדיניות מתוחם שאינה [מוגדרת כראוי: כיצד לקבוע את תצורת המדיניות ' הגנה מפני מידע ' עבור משתמשים ספציפיים באמצעות מדיניות מתוחם](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. אם תיוג אוטומטי אינו פועל עבור Outlook בעת צירוף מסמך המסומן בתווית, ודא `DRMEncryptProperty` שאינו מוגדר כמתואר כאן: [הגדרות הרישום של IRM עבור אבטחה](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. אם השתמשת [בסוגי המידע המוכללים](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) עבור מדיניות ' הגנת מידע תכלת ', ודא שהתוכן תואם לתבנית הצפויה.
5. ודא שהתווית מוגדרת כראוי עבור **אוטומטי** או **מומלץ**. (תיוג**אוטומטי** זמין עבור כל יישומי office, בעוד **המומלץ** זמין עבור כל יישומי office למעט Outlook.)
6. אין באפשרותך להשתמש בסיווג אוטומטי עבור מסמכים ואימיילים שסומנו בעבר באופן ידני או בעבר באופן אוטומטי המסומן בסיווג גבוה יותר.  לקבלת מידע נוסף, ראה: [החלת תוויות אוטומטיות או מומלצות](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. אם אתם עדיין חווים בעיות, אנא אספו את יומני הלקוחות של הגנת המידע התכלת וחברו את היומנים המיוצאים לכרטיס התמיכה שלכם. לייצוא יומני הגנת מידע תכלת:
    - פתח מסמך של Office או צור מייל חדש ב-Outlook.
    - לחץ **Protect/Sensitivity**על  >  **עזרה ומשוב של הגנה**/רגישות.
    - לחץ על **ייצוא יומני רישום**.
    - שמור את יומני הרישום בבחירת המיקום שלך וצרף אותם לבקשת השירות שלך.

לקבלת מידע נוסף, ראה:

- [כיצד להגדיר תנאים לסיווג אוטומטי ומומלץ להגנת מידע תכלת](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [מדריכי ' כיצד לעשות ' עבור תרחישים נפוצים המשתמשים בהגנה על מידע תכלת](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [סקירת התיעוד של הגנת מידע תכלת](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [סקירת מנויים ותכונות של הגנת מידע תכלת](https://azure.microsoft.com/pricing/details/information-protection)
- [דרישות להגנה מפני מידע תכלת](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [הדרכה מהירה עבור הגנת מידע תכלת](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [הורד את לקוח הגנת מידע תכלת](https://www.microsoft.com/download/details.aspx?id=53018)
