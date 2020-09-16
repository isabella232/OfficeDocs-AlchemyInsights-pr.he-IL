---
title: 'AIP: פריטי מדיניות אינם מתנהגים כמצופה'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663190"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: פריטי מדיניות אינם מתנהגים כמצופה

הגנה על מידע תכלת: פריטי מדיניות אינם מתנהגים כמצופה, עיין בסעיפים הבאים לקבלת הנחיות מומלצות עבור בעיות מדיניות שונות:

1. אם אתה נתקל בבעיות עם סימונים חזותיים, עיין בנושא [החלת סימונים חזותיים](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. אם אתה נתקל בבעיות בהוספת תוויות אוטומטיות, עיין בנושא [קביעת התצורה של תנאים לסיווג אוטומטי ומומלץ להגנת מידע של תכלת](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) [ומידע אודות סוגי המידע הרגישים](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. אם אתה נתקל בבעיות עם הגנה מקורית/Pfile, עיין [בתצורה של תצורת הקובץ API](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. בדוק אם אתה משתמש בפריטי מדיניות הנמצאים בטווח שאינו [מוגדר כהלכה: כיצד לקבוע את התצורה של מדיניות הגנת המידע של תכלת עבור משתמשים ספציפיים באמצעות מדיניות בטווח](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
5. אם התווית האוטומטית אינה פועלת עבור Outlook בעת צירוף מסמך עם תוויות, ודא ש-DRMEncryptProperty אינו מוגדר כמתואר כאן: [הגדרות רישום של IRM עבור אבטחה](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

אם אתה עדיין נתקל בבעיות, אסוף את יומני הלקוחות של הגנה על מידע תכלת וצרף את יומני הרישום המיוצא לכרטיס זה.

1. פתח מסמך Office או צור הודעת דואר אלקטרוני חדשה ב-Outlook.
2. לחץ על **הגנה/**  >  **עזרה ומשוב**על רגישות.
3. לחץ על **יצא יומני רישום**.
4. שמור את יומני הרישום בבחירת המיקום שלך וצרף אותם לבקשת שירות זו.

משאבים נוספים:

- [כיצד להגדיר תווית עבור סימונים חזותיים עבור הגנה על מידע תכלת](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [סקירת התיעוד של הגנה על מידע תכלת](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [שימוש בתוויות רגישות ביישומי Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

