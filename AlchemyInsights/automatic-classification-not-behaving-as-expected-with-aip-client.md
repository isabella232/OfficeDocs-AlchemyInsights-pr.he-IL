---
title: סיווג אוטומטי אינו מתנהג כצפוי עם לקוח AIP
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4373"
ms.openlocfilehash: b7ab09fe8430a54dacf2cd1ba076414a5f562541
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820899"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>סיווג אוטומטי אינו מתנהג כצפוי עם לקוח AIP

סיווג אוטומטי אינו מתנהג כצפוי, השתמש בקווים המנחים המומלצים הבאים:

1. אם אתה נתקל בבעיות בתיוג אוטומטי, ראה כיצד לקבוע את התצורה של תנאים עבור סיווג אוטומטי ומומלץ עבור [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ומה סוגי המידע [הרגישים מחפשים](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. בדוק אם אתה משתמש במדיניות טווח שלא נקבעה כראוי: כיצד לקבוע את התצורה של מדיניות Azure Information Protection עבור משתמשים ספציפיים באמצעות [פריטי מדיניות בטווח.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
3. אם תיוג אוטומטי אינו פועל עבור Outlook בעת צירוף מסמך עם תוויות, ודא שהוא אינו מוגדר `DRMEncryptProperty` כמתואר כאן: הגדרות [הרישום של IRM עבור אבטחה.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)
4. אם השתמשת [בסוגי המידע המוכללים עבור מדיניות](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) Azure Information Protection, ודא שהתוכן שלך תואם לתבנית הצפויה.
5. ודא שהתווית מוגדרת כראוי עבור **אוטומטי או** **מומלץ.** (**תיוג** אוטומטי זמין עבור כל יישומי Microsoft  365, בעוד שמומלץ זמין עבור כל יישומי Microsoft 365 למעט עבור Outlook.)
6. לא ניתן להשתמש במיון אוטומטי עבור מסמכים והודעות דואר אלקטרוני עם תווית ידנית או בעבר עם סיווג גבוה יותר.  לקבלת מידע נוסף, ראה: [אופן ההחלה של תוויות אוטומטיות או מומלצות](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. אם אתה עדיין נתקל בבעיות, אסוף יומני לקוח של Azure Information Protection וצרף את יומני הרישום המיוצאים לכרטיס התמיכה שלך. כדי לייצא יומנים של Azure Information Protection:
    - פתח מסמך Office או צור הודעת דואר אלקטרוני חדשה ב- Outlook.
    - לחץ **על הגנה/רגישות**  >  **עזרה ומשוב.**
    - לחץ **על ייצוא יומני רישום**.
    - שמור את יומני הרישום במיקום שלך וצרף אותם לבקשת השירות שלך.

לקבלת מידע נוסף, ראה:

- [כיצד להגדיר תנאים עבור סיווג אוטומטי ומומלץ עבור Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [מדריכי 'כיצד לעשות' עבור תרחישים נפוצים משתמשים ב- Azure Information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [סקירת התיעוד של Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [סקירת מנויים ותכונות של Azure Information Protection](https://azure.microsoft.com/pricing/details/information-protection)
- [דרישות עבור Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [ערכת לימוד להתחלה מהירה עבור Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [הורד את לקוח Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
