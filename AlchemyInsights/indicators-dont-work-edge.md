---
title: מחוונים לא פועלים באמצעות דפדפן Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676242"
---
# <a name="indicators-dont-work-using-edge-browser"></a>מחוונים לא פועלים באמצעות דפדפן Edge

לאחר יצירת מחוון, הוא אינו מכובד על-ידי Edge (Smartscreen). לקבלת מידע נוסף, ראה [יצירת מחוונים עבור כתובות URL וכתובות URL/תחומים.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)

## <a name="step-1-ensure-the-following"></a>שלב 1: ודא שהפעולות הבאות

- ודא כי המחוון נכון (אין שגיאות הקלדה ב- IP/URL, הפעולה הנכונה, קבוצות ה- RBAC הנכונות).
- המתן שעתיים לפחות לאחר יצירת המחוון כדי לקחת בחשבון כל השהיה אפשרית.
- ודא שהמערכת(ים) המשולבות ב- Microsoft Defender עבור נקודת קצה.
- ודא שמערכת(ים) זו יכולה לקיים תקשורת עם הענן.
- ודא ש- Smartscreen זמין וניתן להגיע אליו על-ידי [מחשב שלך](https://demo.smartscreen.msft.net).

## <a name="step-2-troubleshoot-the-potential-issue"></a>שלב 2: פתרון הבעיה הפוטנציאלית

- ודא שהלקוח לעמוד בדרישות. לקבלת פרטים, ראה [יצירת מחוונים עבור כתובות URL וכתובות URL/תחומים](/microsoft-365/security/defender-endpoint/indicator-ip-domain).
- ודא שאתה משתמש בגירסה העדכנית ביותר של דפדפן Edge. כדי לגלות את הגירסה העדכנית ביותר, [ראה גלה איזו גירסה Microsoft Edge שלך.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)
- הפעל מחדש את דפדפן Edge.
- נווט אל האתר שעבורו הגדרת מחוון. אם האתר אינו מופיע כצפוי, המשך לשלב 3. 

## <a name="step-3-collect-data"></a>שלב 3: איסוף נתונים

- איסוף **נתוני אבחון של MDEClientAnalyzer.** לקבלת הוראות, ראה [בעיות עם מחשבים ל- Microsoft Defender עבור נקודת קצה.](issues-with-onboarding-machines.md)
- אם אתה מרגיש בנוח להתקין ולאסוף מעקב אחר Fiddler, ראה [Telerik Fiddler](http://www.telerik.com/fiddler).
- אם אתה מעדיף הדרכה מהתמיכה של Microsoft, בחר את סמל התמיכה להלן כדי לפתוח מקרה תמיכה.
