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
ms.openlocfilehash: 2a48a49ec52a585e450edf448bc9203cd9c3f935
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: he-IL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326262"
---
# <a name="indicators-dont-work-using-edge-browser"></a>מחוונים לא פועלים באמצעות דפדפן Edge

לאחר יצירת מחוון, הוא אינו מכובד על-ידי Edge (Smartscreen). לקבלת מידע נוסף, ראה [יצירת מחוונים עבור כתובות URL וכתובות URL/תחומים.](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)

## <a name="step-1-ensure-the-following"></a>שלב 1: ודא שהפעולות הבאות

- ודא כי המחוון נכון (אין שגיאות הקלדה ב- IP/URL, הפעולה הנכונה, קבוצות ה- RBAC הנכונות).
- המתן שעתיים לפחות לאחר יצירת המחוון כדי לקחת בחשבון כל השהיה אפשרית.
- ודא שהמערכת(ים) המשולבות ב- Microsoft Defender עבור נקודת קצה.
- ודא שמערכת(ים) זו יכולה לקיים תקשורת עם הענן.
- ודא ש- Smartscreen זמין וניתן להגיע אליו על-ידי [מחשב שלך](https://demo.smartscreen.msft.net).

## <a name="step-2-troubleshoot-the-potential-issue"></a>שלב 2: פתרון הבעיה הפוטנציאלית

- ודא שהלקוח לעמוד בדרישות. לקבלת פרטים, ראה [יצירת מחוונים עבור כתובות URL וכתובות URL/תחומים](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain).
- ודא שאתה משתמש בגירסה העדכנית ביותר של דפדפן Edge. כדי לגלות את הגירסה העדכנית ביותר, [ראה גלה איזו גירסה של Microsoft Edge יש לך](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).
- הפעל מחדש את דפדפן Edge.
- נווט אל האתר שעבורו הגדרת מחוון. אם האתר אינו מופיע כצפוי, המשך לשלב 3. 

## <a name="step-3-collect-data"></a>שלב 3: איסוף נתונים

- איסוף **נתוני אבחון של MDEClientAnalyzer.** לקבלת הוראות, ראה [בעיות עם מחשבים ל- Microsoft Defender עבור נקודת קצה.](issues-with-onboarding-machines.md)
- אם אתה מרגיש בנוח להתקין ולאסוף מעקב אחר Fiddler, ראה [Telerik Fiddler](http://www.telerik.com/fiddler).
- אם אתה מעדיף הדרכה מהתמיכה של Microsoft, בחר את סמל התמיכה שלהלן כדי לפתוח מקרה תמיכה.
