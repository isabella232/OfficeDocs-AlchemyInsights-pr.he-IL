---
title: 'AIP: פריטי מדיניות אינם מתנהגים כצפוי'
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
- "4780"
ms.openlocfilehash: 90448bf57297ce59ba222efd1927b5de588bfbfdb1206b6403764d7f43fed690
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934294"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: פריטי מדיניות אינם מתנהגים כצפוי

Azure Information Protection: פריטי מדיניות אינם מתנהגים כצפוי, עיין בנושאים הבאים לקבלת קווים מנחים מומלצים עבור בעיות מדיניות שונות:

1. אם אתה נתקל בבעיות עם סימונים חזותיים, עיין [בעת החלת סימונים חזותיים](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. אם אתה נתקל בבעיות בתיוג אוטומטי, עיין באופן קביעת התצורה של תנאים עבור סיווג אוטומטי ומומלץ עבור [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ומה סוגי המידע [הרגישים מחפשים](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. אם אתה נתקל בבעיות בהגנה מקורית/Pfile, עיין בתצורת [ה- API של הקובץ](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. בדוק אם אתה משתמש במדיניות טווח שלא נקבעה כראוי: כיצד לקבוע את התצורה של מדיניות Azure Information Protection עבור משתמשים ספציפיים באמצעות [פריטי מדיניות בטווח.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
5. אם סימון אוטומטי אינו פועל עבור Outlook בעת צירוף מסמך עם תוויות, ודא ש- DRMEncryptProperty אינו מוגדר כמתואר כאן: הגדרות [הרישום של IRM עבור אבטחה.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)

אם אתה עדיין נתקל בבעיות, אסוף יומני לקוח של Azure Information Protection וצרף את יומני הרישום המיוצאים לכרטיס זה.

1. פתח מסמך Office או צור הודעת דואר אלקטרוני חדשה ב- Outlook.
2. לחץ **על הגנה/רגישות**  >  **עזרה ומשוב.**
3. לחץ **על ייצוא יומני רישום**.
4. שמור את יומני הרישום במיקום שלך וצרף אותם לבקשת שירות זו.

משאבים נוספים:

- [כיצד להגדיר תווית עבור סימונים חזותיים עבור Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [סקירת התיעוד של Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [שימוש בתוויות רגישות Microsoft 365 יישומים](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

